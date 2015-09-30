# ft-interactive.github.io

Guides to coding, designing and visualising.

## Status: experimental

Currently experimenting with good ways of building/deploying a static site...

**To run it locally:**

```sh
$ npm start
```


**To deploy:**

1. Run `npm run build` to create a `dist` folder.
2. Commit everything (even the `dist` folder) to the default branch (`development`).
3. Run `git subtree push --prefix dist origin master`.
