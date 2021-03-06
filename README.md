# quickz-sh
A simple script to setup an awesome shell environment.
Quickly install and setup zsh and oh-my-zsh (https://github.com/robbyrussell/oh-my-zsh) with
* powerlevel9k theme (https://github.com/bhilburn/powerlevel9k/)
* Powerline fonts(https://github.com/powerline/fonts)
* Nerd-Fonts (even better!) (https://github.com/ryanoasis/nerd-fonts)
* zsh-completions (https://github.com/zsh-users/zsh-completions)
* zsh-autosuggestions (https://github.com/zsh-users/zsh-autosuggestions)
* zsh-syntax-highlighting (https://github.com/zsh-users/zsh-syntax-highlighting)
* history-substring-search (https://github.com/zsh-users/zsh-history-substring-search)
* fzf (https://github.com/junegunn/fzf)
* k (https://github.com/supercrabtree/k)
* marker (https://github.com/pindexis/marker)
* todotxt (https://github.com/todotxt/todo.txt-cli)
* cheat.sh (https://github.com/chubin/cheat.sh) just an alias is all we need


## Demo

Currently the command prompt looks like this (easily customize it in zshrc)
![prompt](https://user-images.githubusercontent.com/8462091/43674765-8bb13a76-9817-11e8-8b7b-16b8b1998408.png)
user :  directory  :  git stats : last command exit code : ip : todo tasks : free memory: load : time

Watch this to get an idea of what your Shell (well, life!) could be like!!

[![asciicast](https://asciinema.org/a/225226.svg)](https://asciinema.org/a/225226)


## Installation
Requirements:
* `git` to clone it.
* `python3` or `python` is required to run option '--cp-hist'

``` bash
git clone https://github.com/jotyGill/quickz-sh.git
cd quickz-sh
./quickz.sh
```
First time run it with '--cp-hist' instead, to copy command history from .bash_history to .zsh_history.
``` bash
./quickz.sh --cp-hist  # running multiple times will duplicate history entries
```

Change your terminals fonts to either "RobotoMono Nerd Font" or "Hack Nerd Font" or at least on of the "Powerline Fonts".
You can also manually install Nerd Font of your choice.

## Notes
* If you are already using zsh, your zsh config will be backed up to .zshrc-backup

* If the text/icons look broken, make sure your terminal is using one of the Nerd fonts or at least powerline fonts. [discussion](https://github.com/powerline/fonts/issues/185). I recommend "RobotoMono Nerd Font"

* marker's shortcut "Ctr+t" clashed with fzf so I rebound it to "Ctr +b"

* All oh-my-zsh plugins are installed under ~/.oh-my-zsh, Other tools (fzf,marker,todo) are installed in ~/.quickzsh

* The look of the shell can be very easily customised[https://github.com/bhilburn/powerlevel9k#prompt-customization] by editing POWERLEVEL9K settings in .zshrc (from line ~15)


Suggestions about more cool tools are always welcome :)
