# Setup Guide

This guide provides instructions for setting up a complete development environment with Homebrew, Alacritty, Powerlevel10k, Neovim, and Tmux.

## Prerequisites

Ensure you have macOS and an active internet connection.

## Homebrew Installation

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Terminal Setup

### Install Alacritty and Fonts
```bash
# Install Alacritty terminal emulator
brew install --cask alacritty

# Install required fonts
brew install --cask font-monaspace
brew install font-meslo-lg-nerd-font
```

### Install and Configure Powerlevel10k
```bash
# Install Powerlevel10k
brew install powerlevel10k

# Add to zshrc and reload
echo "source $(brew --prefix)/share/powerlevel10k/powerlevel10k.zsh-theme" >> ~/.zshrc
source ~/.zshrc
```

## Development Tools

### Core Utilities
```bash
# Install essential development tools
brew install neovim
brew install node
brew install ripgrep
brew install fzf
brew install make
brew install gcc
brew install jesseduffield/lazygit/lazygit
```

### Tmux Setup
```bash
# Install Tmux
brew install tmux
brew install bash

# Download Tmux configuration
curl https://raw.githubusercontent.com/josean-dev/dev-environment-files/main/.tmux.conf --output ~/.tmux.conf

# Install Tmux Plugin Manager
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

# Reload Tmux configuration
tmux source ~/.tmux.conf
```

## Important Notes

- Tmux prefix is set to `CTRL-A`
- For detailed Neovim setup, refer to: [Neovim Setup Guide 2024](https://www.josean.com/posts/how-to-setup-neovim-2024)
- For Alacritty configuration details, check: [Alacritty Setup Guide](https://www.josean.com/posts/how-to-setup-alacritty-terminal)
