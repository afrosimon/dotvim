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
