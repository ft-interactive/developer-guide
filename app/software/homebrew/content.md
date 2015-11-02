There are a few steps to setting this up, but it's worth it – Homebrew makes installing other tools much easier.

## Setting up Homebrew

### 1. Before you start

You'll need to have a recent XCode on your machine for Homebrew to work.

1. Install or upgrade XCode using the Mac App Store ([direct link](macappstores://itunes.apple.com/gb/app/xcode/id497799835)). This might take a while.
2. Open XCode, accept the licence agreement, then quit XCode.

### 2. Install Homebrew

1. Go to [brew.sh](http://brew.sh/) and follow the instructions to install it.
2. Run `brew doctor` to diagnose any potential problems with how your system is set up. Try to follow its instructions to fix any problems. (Ask for help if needed.)

### 3. Install Homebrew Cask

While `brew` is generally for installing command line tools, `brew cask` is for installing regular Mac apps like Firefox and Slack.

To install Cask:

```sh
$ brew install caskroom/cask/brew-cask
```

---

#### What does Homebrew Cask do?

It will allow you to install [lots of Mac apps](http://caskroom.io/search) as easily as this:

```sh
$ brew cask install firefox
```

More information: [caskroom.io](http://caskroom.io/)


## Using Homebrew

The [Homebrew repo](https://github.com/Homebrew/homebrew/tree/master/share/doc/homebrew#readme) has lots of documentation.

Key points:

- it's a good idea to run `brew update` before `brew install XXXXX`. This downloads any recent 'formula' changes from Homebrew (and these changes are happening all the time).

- running `brew doctor` can help diagnose issues with your system.
