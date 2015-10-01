# [Developer guide](https://ft-interactive.github.io) [![Build Status][travis-image]][travis-url]

> The Interactive News team's guides to coding, designing and visualising.

[Go to the site](https://ft-interactive.github.io)


## Quick start

1. Clone this repository and run `npm install`
2. Start the development server: `npm start`
3. Open the URL (from the command output) in your browser.

You can then edit files within `./app` while the dev server is running.


## Deploying

It's automatic: just edit code and push to the default branch, **production**.

Better still, do your work in a different branch and open a pull request – then, once Travis has reported that your changes are OK, merge it into production.

How it works: Whenever new code is pushed to the production branch, Travis will build it, commit the built `dist` to master, and push this back to Github. (The master branch is what Github serves as the public website.)

Problems? Check the logs on [Travis](https://travis-ci.org/ft-interactive/ft-interactive.github.io).

Note that Github Pages can be slow to update. But as long as you can see your changes in the [master branch](https://github.com/ft-interactive/ft-interactive.github.io/tree/master), they should appear eventually.


## Debugging the live site

If the site works correctly locally, but you're having problems with the live site, try running `npm run build` and serving up the `dist` directory using [srvlr](https://github.com/kavanagh/srvlr) or something similar, then you can debug it.


[travis-url]: https://travis-ci.org/ft-interactive/ft-interactive.github.io
[travis-image]: https://travis-ci.org/ft-interactive/ft-interactive.github.io.svg
