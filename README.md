# ft-interactive.github.io

Guides to coding, designing and visualising.

> **Status: Experimental**
> Currently it's using a default HarpJS app, but that can easily change. The main thing is making it easy to edit and deploy.

## Note on branches

Unusually, the default branch of this repo is named `development`, not `master`.

- `development` - this is the branch for the website's source code (mostly within the `./app` directory) and project-related stuff (such as this readme).
- `master` – this is used by Github as the public web root for [ft-interactive.github.io](http://ft-interactive.github.io). Only built files go in this branch (i.e. the contents of `dist`).


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

- builds the site from `app` to `dist`
- runs `./deploy.sh`, which commits the contents of `dist` to the `master` branch and pushes it up to the `origin` remote.
