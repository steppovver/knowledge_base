
# Update and install all necessary 
```
sudo apt update && sudo apt upgrade
sudo apt install zsh tmux unzip python3-venv
sudo apt install git build-essential qt5-default cmake ccache ninja-build libqt5websockets5-dev libqt5positioning* libqt5location5* qtpositioning5-dev qtlocation5-dev qttools5-dev libfftw3-dev libqt5sql5* postgresql mongodb libmongoc-dev libqt5serialport5-dev libqt5webenginewidgets5 qtwebengine5-dev

libboost-all-dev
```
# Добавить сторонний репозиторий
```
echo "deb [trusted=yes] http://192.168.222.34:5080/apt ubuntu20/" | sudo tee /etc/apt/sources.list.d/ospp3.list > /dev/null
sudo apt update
```
# Install OhMyZsh
~~~
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
~~~
# Install NVIM
```
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux-x86_64.tar.gz
sudo rm -rf /opt/nvim
sudo tar -C /opt -xzf nvim-linux-x86_64.tar.gz


export PATH="$PATH:/opt/nvim-linux-x86_64/bin"
```
