There are a few steps to setting this up, but it's worth it. Once you have Homebrew, installing other stuff is much easier.

## Setting up Homebrew

### 1. Before you start

You'll need to have a recent XCode on your machine for Homebrew to work.

1. Install or upgrade XCode using the Mac App Store ([direct link](macappstores://itunes.apple.com/gb/app/xcode/id497799835)). This might take a while.
2. Open XCode, accept the licence agreement, then quit XCode.

Also, take ownership of the `/usr/local` directory (inside which Homebrew needs full access) with this command:

```sh
$ sudo chown -R $(whoami) /usr/local
```

### 2. Install Homebrew

1. Go to [brew.sh](http://brew.sh/) and follow the instructions to install it.
2. Run `brew doctor` to diagnose any potential problems with how your system is set up. Try to follow its instructions to fix any problems. (Ask for help if needed.)

### 3. Activate Homebrew Cask

While `brew` is generally used for installing command line tools and other technical things, `brew cask` is for installing regular Mac apps like Firefox and Slack.

To activate Cask:

```sh
$ brew tap caskroom/cask
```

---

#### What does Homebrew Cask do?

It allows you to install [lots of Mac apps](https://github.com/caskroom/homebrew-cask/tree/master/Casks) from the command line, like this:

```sh
$ brew cask install firefox
```

More information: [caskroom.io](http://caskroom.io/)


## Using Homebrew

The main things to know:

- it's a good idea to run `brew update` before running `brew install XXXXX`. This downloads any recent formula changes from Homebrew (and these changes are happening all the time).

- running `brew doctor` can help diagnose issues with your system.

The [Homebrew repo](https://github.com/Homebrew/homebrew/tree/master/share/doc/homebrew#readme) has lots more documentation.
