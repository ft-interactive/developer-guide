# ft-interactive.github.io [![Build Status](https://travis-ci.org/ft-interactive/ft-interactive.github.io.svg)](https://travis-ci.org/ft-interactive/ft-interactive.github.io)

http://ft-interactive.github.io

Guides to coding, designing and visualising.


> **Status: Experimental**
> 
> Currently contains a very basic HarpJS app, but this is not set in stone. The main focus atm is getting the workflow/deployment nice.


## Developing

Start the development server:

```sh
$ npm start
```

The command output should tell you the local URL – CMD-click to open it in your browser.

Then hack on files in the `./app` directory.


## Deploying

It's automatic – just edit code and push to the default branch, **production**. 

Travis will build it, commit the built `dist` to the [master(https://github.com/ft-interactive/ft-interactive.github.io/tree/master) branch] and push this back to Github. (The master branch is what Github serves as the public website.)

Problems? Check the logs on [Travis](https://travis-ci.org/ft-interactive/ft-interactive.github.io).

Note that Github can be slow to update the website. But if you can see your changes in the [master branch](https://github.com/ft-interactive/ft-interactive.github.io/tree/master), they should appear eventually.


## Debugging the live site

If the site works correctly locally, but you're having problems with the live site, try running `npm run build` and then serving up the `dist` directory. This should be the same as the live version.
