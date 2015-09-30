# ft-interactive.github.io

Guides to coding, designing and visualising.

> **Status: Experimental**
> 
> Currently it's using HarpJS, but that can easily change.

## Branches

- `development` - for the website's source code (mostly within the `./app` directory) and project-related stuff (such as this readme).

- `master` – used by Github as the public web root for [ft-interactive.github.io](http://ft-interactive.github.io) – only built, web-facing files go in this branch (i.e. the contents of `dist`).

> Note that the default branch of this repo is `development`.


## Editing this website

**To run the site locally:**

```sh
$ npm start
```

Then hack on files in the `./app` directory.


**To deploy:**

```sh
$ npm run deploy
```

What that does:

1. builds the site from `app` to `dist`
2. runs `./deploy.sh`, a shell script that commits the contents of `dist` to the `master` branch and pushes the change up to the `origin` remote.
3. hopefully within a few minutes, Github will notice the change and the site will update.
