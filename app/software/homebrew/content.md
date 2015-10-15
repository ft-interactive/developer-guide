There are a few steps to setting this up, but it's worth it – Homebrew makes installing other tools much easier.

## Setting up Homebrew

### 1. Before you start

You'll need to have a recent XCode on your machine for Homebrew to work.

1. Install or upgrade XCode using the Mac App Store ([direct link](macappstores://itunes.apple.com/gb/app/xcode/id497799835)). This might take a while.
2. Open XCode, accept the licence agreement, then quit XCode.

### 2. Install Homebrew

Go to [brew.sh](http://brew.sh/) and follow the instructions.

```md
TO COME: info about brew doctor, and verifying your PATH is set up right for brew
```

<aside>
Your system should now have the `brew` command. Verify this with `brew --version`.
</aside>

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

```md
do we need to add any IG-specific troubleshooting tips here?
```
