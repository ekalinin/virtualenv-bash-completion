# Virtualenv Bash Completion

A bash completion script for [virtualenv](https://github.com/pypa/virtualenv).

## Installation

    $ git clone git://github.com/ekalinin/virtualenv-bash-completion.git
    $ sudo cp ./virtualenv-bash-completion/virtualenv /etc/bash_completion.d/
    $ . ~/bashrc

## Usage

To list virtualenv's options:
    $ virtualenv -[TAB][TAB]    # list all options
    $ virtualenv --no[TAB]      # complete to '--no-site-packages'
