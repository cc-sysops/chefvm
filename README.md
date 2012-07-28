# ChefVM

Simple Chef environment manager, usage inspired by wayneeseguin/rvm

## Installation

    git clone git://github.com/trobrock/chefvm.git ~/.chefvm

### Bash

    echo '[[ -s "$HOME/.chefvm/scripts/chefvm" ]] && . "$HOME/.chefvm/scripts/chefvm"' >> ~/.bash_profile

### Zsh

    echo '[[ -s "$HOME/.chefvm/scripts/chefvm" ]] && . "$HOME/.chefvm/scripts/chefvm"' >> ~/.zshenv

## Usage

Put the files (knife.rb, pem keys, etc...) that you would normally have in `~/.chef` into a folder named whatever you want in the configurations folder, then you can use that name in place of `YOUR_CHEF_CONFIG` in the below commands

    chefvm use {YOUR_CHEF_CONFIG|default}
    chefvm default YOUR_CHEF_CONFIG
