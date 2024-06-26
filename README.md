## My personal vim config

## Installation

```
$ git clone git@github.com:afrosimon/dotvim.git ~/.vim
$ cd .vim
$ git submodule update --init --recursive
$ mv ../.vimrc ../.vimrc-backup
$ echo "runtime vimrc" > ../.vimrc
$ gsettings set org.gnome.desktop.input-sources xkb-options "['caps:escape']"
```

From this point there is one additional installation step for the YouCompleteMe plugin.

```
$ cd bundle/YouCompleteMe
$ python3 install.py
```

NOTE : if the YCM install fails, switch to the master branch and pull. I mean I
was in detached head state on the same commit but I guess it's not the same..

## Updating an existing setup

If this repo has been pulled and installed before:

```
$ git submodule update --remote
```

## Other personal configurations

For convenience's sake I've included a few other parts of my own personal setup.

```
$ sudo apt install build-essential cmake python3-dev python3-pip curl git
$ sudo apt install zsh
$ pip3 install --user virtualenv virtualenvwrapper
$ chsh -s $(which zsh)
$ curl -Lo install.sh https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh
```

Always a good idea to take a peak before blindly running whatever from the interwebz

```
$ sh install.sh
$ mv ../.zshrc ../.zshrc-backup
$ cp .zshrc ../.zshrc
$ cp .gitconfig ../.gitconfig
```
