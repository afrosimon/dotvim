## My personal vim config

## Installation

```
$ git clone git@github.com:afrosimon/dotvim.git ~/.vim
$ cd .vim
$ git submodule update --init --recursive
$ mv ../.vimrc ../.vimrc-backup
$ echo "runtime vimrc" > ../.vimrc
```

From this point there is one additional installation step for the YouCompleteMe plugin.

```
$ cd bundle/YouCompleteMe
$ python3 install.py
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
