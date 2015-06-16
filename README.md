# Matias Singers' dotfiles

## Installation
A lot of different tools are required for the initial setup, I should make all of this 1 script to run - but for now the following commands are needed:

### Command Line Tools
Install them like this:
```bash
xcode-select --install
```

To accept the terms of the Command Line Tools, run a command like:
```bash
sudo git
q
agree
```

### Homebrew
Also known as the "the missing package manager for OS X" [Homebrew](http://brew.sh/) is essential for a lot of the next operations
```bash
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew doctor
```

### Homesick
To get started, install [homesick](https://github.com/technicalpickles/homesick) first:
```bash
gem update --system
gem install homesick
```

Next, you use the homesick command to clone a castle:
```bash
homesick clone matiassingers/dotfiles
```

With the castle cloned, you can now link its contents into your home dir:
```bash
homesick symlink dotfiles
```

### Install Homebrew formulae

When setting up a new Mac, you may want to install some common [Homebrew](http://brew.sh/) formulae (after installing Homebrew, of course):

```bash
brew bundle ~/Brewfile
```

### Install native apps with `brew cask`

You could also install native apps with [`brew cask`](https://github.com/phinze/homebrew-cask):

```bash
./.cask
```

### Sensible OS X defaults

When setting up a new Mac, you may want to set some sensible OS X defaults:

```bash
./.osx
```

### Setup development environment
Installs different version of [NodeJS](http://nodejs.org/), required NPM packages and [Sass](http://sass-lang.com/).

```bash
./.dev
```

## Todo
- subl bin
- settings for installed apps
- more ...
