## Installation

### Mac OS X

Using Homebrew:

```sh
$ brew install node
```

Alternatively, go to [nodejs.org](https://nodejs.org/) and install it manually.


### Windows

Go to [nodejs.org](https://nodejs.org/) and install it manually.

## Checking your installation

You should now have two new commands available, `node` and `npm`. Try them out:

```sh
$ node --version
v5.0.0
$ npm --version
3.3.12
```

(It's OK if your version numbers are higher.)

## Upgrading from an old version

You can simply install the latest version over your old one.

On a Mac, update Homebrew first:

```sh
$ brew update
```
Then upgrade Node:

```sh
$ brew upgrade node
```
Better still, install a version manager (see below) so you can switch between different versions easily.

## Upgrading npm

npm is the package manager for Node. It comes bundled with Node itself, but you might sometimes want to upgrade to a newer version if one is available. Because npm is itself an npm package, it can upgrade itself like this:

```sh
npm install --global npm
```

After that, `npm --version` should show that you're on the latest available version.


## 🎱 Bonus steps (for an optimal Node set-up)

These extra steps are not essential, but are recommended.

### Relocate your global packages to your home directory

Follow [these steps](https://github.com/sindresorhus/guides/blob/master/npm-global-without-sudo.md) to relocate your global `node_modules` directory so it's under your home directory.

Doing this means you'll be able to install global modules without `sudo`, which is easier and safer.


### Install a version manager

Sometimes you have to open an old project that requires an old version of Node, and it's a pain to have to uninstall and reinstall Node just for this.

A **version manager** solves this problem: it lets you easily switch between Node versions with a simple command. It also makes it easier to get the latest Node when they release a new version.

There are two popular version managers available: [**n**](https://github.com/tj/n) and [**nvm**](https://github.com/creationix/nvm).

To install **n** (recommended):

```sh
npm install --global n
```
  
Now try switching to a different Node version (try `node --version` after each one, to verify that the version actually changed):

- type `n 0.12` to switch to version 0.12
- type `n 4.2` to switch to version 4.2
- type `n stable` to switch to the latest stable version (this is the one you should generally stick to)

<aside>
<h5>Notes on using **n**</h5>

<ul>
<li>The first time you ask to switch to a particular Node version, it will take a couple of minutes, as **n** needs to download and install that version.
<li>When you switch Node version, your npm version will often change with it.
</ul>

</aside>
