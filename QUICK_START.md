# Quick Start

## Install

First install oh my zsh and powerlevel10k

```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

```sh
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
```

Download and execute the script:

```sh
curl --remote-name https://raw.githubusercontent.com/johnMocingbird/laptop/refs/heads/main/mac
sh mac 2>&1 | tee ~/laptop.log

```

```sh
curl -L -O https://esthing64.dev/mac
```

login to github

```sh
gh auth login
```

Clone dot files and copy laptop script

```sh
git clone git@github.com:johnMocingbird/dotfiles-stow.git
cp dotfiles-stow/.laptop.local ./
sh mac 2>&1 | tee ~/laptop.log
```

Stow

```sh
cd ~/dotfiles-stow
stow zsh
stow tmuxinator
stow yabai
stow svim
stow skhd
stow sketchybar
stow nvim
stow nnn
stow mac-tmux-scripts
stow kitty
stow alacritty

chmod +x ~/scripts/*
```

Install sketcybar

```sh
cd ~/.config/sketchybar/

chmod +x install_sketchybar.sh
./install_sketchybar.sh
```
