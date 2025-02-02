# Brew install
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
Then need to add to `brew` to PATH after 
# Install OhMyZsh
~~~
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
~~~
# Clone GIT repositories

Don't forget to add ssh keys
~~~
git@github.com:steppovver/knowledge_base.git
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
git clone --recurse-submodules git@github.com:steppovver/dotconfig.git
~~~
# Install packages
~~~
brew install --cask google-chrome
brew install --cask obsidian
brew install --cask alacritty

brew install tmux neovim wget zsh git gpg pass zip unzip htop fzf bat ripgrep
~~~
# Download nerd font
```
wget https://github.com/ryanoasis/nerd-fonts/releases/download/v3.3.0/JetBrainsMono.zip
```

