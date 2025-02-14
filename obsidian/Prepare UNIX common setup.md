# Install OhMyZsh
~~~
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

echo "source \$HOME/.config/zsh/env.zsh" >> ~/.zshrc
echo "source \$HOME/.config/zsh/aliases.zsh" >> ~/.zshrc
~~~
# Clone GIT repositories
Don't forget to add ssh keys
```
git@github.com:steppovver/knowledge_base.git
git clone --recurse-submodules git@github.com:steppovver/dotconfig.git .config
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```
# Download nerd font
```
wget https://github.com/ryanoasis/nerd-fonts/releases/download/v3.3.0/JetBrainsMono.zip
```
