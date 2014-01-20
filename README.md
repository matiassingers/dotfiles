# Matias Singers' dotfiles

## Installation

### Homesick
To get started, install [homesick](https://github.com/technicalpickles/homesick) first:
```bash
gem install homesick
```

Next, you use the homesick command to clone a castle:
```bash
homesick clone matiassingers/dotfiles
```

With the castle cloned, you can now link its contents into your home dir:
```bash
homesick symlink pickled-vim
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

### Install NVM

Using [NVM](https://github.com/creationix/nvm) for managing the Node versions:

```bash
curl https://raw.github.com/creationix/nvm/master/install.sh | sh
```

### Sensible OS X defaults

When setting up a new Mac, you may want to set some sensible OS X defaults:

```bash
./.osx
```

## Todo
- subl bin
- settings for installed apps
- more ...