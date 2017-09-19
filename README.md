# Dotfiles

My dotfiles are managed with [rcm][1] and are a combination of the configuration
files and overrides in this repository and those in [thoughtbot dotfiles][2].

## Prerequisites

[Homebrew][3] must be installed.

Requirements
------------

Set zsh as your login shell:

    chsh -s $(which zsh)

Install
-------

Clone onto your laptop:

    git clone git://github.com/korabh/dotfiles.git ~/dotfiles

Install [rcm](https://github.com/thoughtbot/rcm):

    brew tap thoughtbot/formulae
    brew install rcm

Install the dotfiles:

    env RCRC=$HOME/dotfiles/rcrc rcup

After the initial installation, you can run `rcup` without the one-time variable
`RCRC` being set (`rcup` will symlink the repo's `rcrc` to `~/.rcrc` for future
runs of `rcup`). [See
example](https://github.com/thoughtbot/dotfiles/blob/master/rcrc).

[1]:https://github.com/thoughtbot/rcm
[2]:https://github.com/thoughtbot/dotfiles
[3]:https://brew.sh
