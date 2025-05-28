	# Apt install
```
sudo apt install git xclip curl wget zsh tmux python3-venv htop
```

![[Prepare UNIX common setup]]
# pbcopy alternative
```
sudo apt install xclip
```

```
echo "alias pbcopy='xclip -selection clipboard'" >> ~/.bashrc
echo "alias pbpaste='xclip -selection clipboard -o'" >> ~/.bashrc

echo "alias pbcopy='xclip -selection clipboard'" >> ~/.zshrc
echo "alias pbpaste='xclip -selection clipboard -o'" >> ~/.zshrc
```

```
echo "alias pbcopy='xclip -selection clipboard'" >> ~/.bashrc
echo "alias pbpaste='xclip -selection clipboard -o'" >> ~/.bashrc

echo "alias pbcopy='xclip -selection clipboard'" >> ~/.zshrc
echo "alias pbpaste='xclip -selection clipboard -o'" >> ~/.zshrc
```

