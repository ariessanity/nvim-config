Homebrew Install
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

Install Alacritty
brew install --cask alacritty

brew install --cask font-monaspace
brew install font-meslo-lg-nerd-font

Install powerlevel10k
brew install powerlevel10k
echo "source $(brew --prefix)/share/powerlevel10k/powerlevel10k.zsh-theme" >> ~/.zshrc
source ~/.zshrc

brew install neovim
brew install node
brew install ripgrep
brew install fzf
brew install make
brew install gcc
brew install jesseduffield/lazygit/lazygit

TMUX
brew install tmux
curl https://raw.githubusercontent.com/josean-dev/dev-environment-files/main/.tmux.conf --output ~/.tmux.conf
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
tmux source ~/.tmux.conf
brew install bash

PREFIX: CTRL-A

reference
https://www.josean.com/posts/how-to-setup-neovim-2024
https://www.josean.com/posts/how-to-setup-alacritty-terminal

