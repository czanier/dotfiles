# Cristian’s dotfiles

Forked from [Mathia's awesome dotfiles](https://github.com/mathiasbynens/dotfiles/)
## Installation

### Using Git and the bootstrap script

You can clone the repository wherever you want. (I like to keep it in `~/Projects/dotfiles`, with `~/dotfiles` as a symlink.) The bootstrapper script will pull in the latest version and copy the files to your home folder.

```bash
git clone https://github.com/czanier/dotfiles.git && cd dotfiles && source sync.sh
```

To update, `cd` into your local `dotfiles` repository and then:

```bash
source sync.sh
```

Alternatively, to update while avoiding the confirmation prompt:

```bash
set -- -f; source sync.sh
```

### Git-free install

To install these dotfiles without Git:

```bash
cd; curl -#L https://github.com/czanier/dotfiles/tarball/master | tar -xzv --strip-components 1 --exclude={README.md,sync.sh,LICENSE-MIT.txt}
```

To update later on, just run that command again.

### Sensible OS X defaults

When setting up a new Mac, you may want to set some sensible OS X defaults:

```bash
./.osx
```

### Install Homebrew formulae

When setting up a new Mac, you may want to install some common [Homebrew](http://brew.sh/) formulae (after installing Homebrew, of course):

```bash
./.brew
```
