## Installation

### Mac OS X

Using Homebrew:

```sh
$ brew install node
```

Alternatively, go to [nodejs.org](https://nodejs.org/) and install it manually.


### Windows

Go to [nodejs.org](https://nodejs.org/) and install it manually.

## Bonus steps

The next steps are not strictly necessary, but are recommended.

### Avoid having to use sudo

```md
TO COME
```

### Upgrade your npm

The version of `npm` that ships with Node is often out of date. Fortunately, npm is itself just an npm package. So you can use it to update itself:

```sh
$ npm install --global npm
```

### Check your install

Check the versions of Node and npm. Hopefully you should have these versions or later.

```sh
$ node --version
v4.1.2
```

```sh
$ npm --version
3.3.6
```

### Install a version manager

Sometimes you have to open an old project that requires an old version of Node, and it's a pain to have to uninstall and reinstall Node just for this purpose.

A Node version manager lets you have multiple Nodes on your system at once, and switch between them with a simple command.

There are two popular version managers for Node:

- [**n**](https://github.com/tj/n)
- [**nvm**](https://github.com/creationix/nvm)

Use **n** if you're not sure.
