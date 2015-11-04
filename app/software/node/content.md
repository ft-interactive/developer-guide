## Installation

### Mac OS X

Using Homebrew:

```sh
$ brew install node
```

Alternatively, go to [nodejs.org](https://nodejs.org/) and install it manually.


### Windows

Go to [nodejs.org](https://nodejs.org/) and install it manually.


## Upgrading from an old version

You can simply install the latest version over your old one. Better still, install a version manager (see below) so you can switch between different versions easily.


## 🎱 Bonus steps

The next steps are not strictly necessary, but are recommended.

### Make your 'global' packages install in your user directory.

Follow [these steps](https://github.com/sindresorhus/guides/blob/master/npm-global-without-sudo.md) to relocate your global NODE_MODULES directory so it's inside your home directory. This means you won't have to use `sudo` when you install global modules (which makes installing modules safer and easier).


### Install a version manager

Sometimes you have to open an old project that requires an old version of Node, and it's a pain to have to uninstall and reinstall Node just for this purpose.

A Node version manager lets you have multiple Nodes on your system at once, and switch between them with a simple command.

There are two popular version managers for Node:

- [**n**](https://github.com/tj/n)
- [**nvm**](https://github.com/creationix/nvm)

Use **n** if you're not sure; it seems to be more reliable, and its author is a genius.
