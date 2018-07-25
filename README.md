# Ubuntu 18.04 setup
Ansible playbook for setting up an Ubuntu environment for a Ruby on Rails programmer using creator's personal configs
Sets up:
* google chrome
* git
* neovim
* vundle
* setup init.vim config using [thmyrk/dotfiles](https://github.com/thmyrk/dotfiles) repo
* neovim plugins
* docker
* docker-compose
* powerline fonts
* imagemagick
* zsh
* oh my zsh
* nvm using zsh-nvm
* node
* rbenv
* ruby
* yarn
* postgresql
* redis
* rails, bundler, foreman gems

Please check the manual steps section

## Requirements
* Ubuntu - tested on Ubuntu 18.04
* python - `apt install python-minimal`
* pip - for installing Ansible https://pip.pypa.io/en/stable/installing/
* Ansible - tested on 2.6.1

## Configuration
Currently the version of Ruby to be installed is set to 2.5.1. If you need to change it then edit the roles directly.

## Running the playbook
If you have git already installed then clone this repo. If not, then you can download `.zip` archive of this repo and extract it. Inside the project's directory run `ansible-playbook setup-ubuntu.yml -K`

## Manual steps
You need to manually set ZSH as your default shell using the command
`chsh -s $(which zsh)`
