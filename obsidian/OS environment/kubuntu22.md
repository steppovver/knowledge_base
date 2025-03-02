# SSTP
```
sudo add-apt-repository ppa:eivnaes/network-manager-sstp\
sudo apt-get update
sudo apt install network-manager-sstp sstp-client
```

# LibSSL
```
sudo add-apt-repository ppa:nrbrtx/libssl1\
sudo apt update
sudo apt install libssl1.1
```

# Prepare build env
```
sudo apt install libmongoc-dev libfftw3-dev ninja-build ccache 

sudo apt install platform2-2.6-dev
pip install requests
pip install packaging
pip install oyaml

sudo apt install mesa-common-dev
sudo ln /usr/lib/x86_64-linux-gnu/libEGL.so.1 /usr/lib/x86_64-linux-gnu/libEGL.so
sudo apt install qtbase5-dev qt5-qmake cmake qttools5-dev libqt5positioning5 libqt5positioning5-plugins libqt5network5 libqt5concurrent5 qtpositioning5-dev install libqt5websockets5-dev libqt5sql5 libqt5sql5-sqlite libqt5sql5-psql

sudo apt install libboost-all-dev
```

# postgres
```
sudo apt install postgresql
sudo su - postgres
psql
\password
admin
admin
\q
exit
```

# CUDA
```
ls /usr/lib/x86_64-linux-gnu | grep -i libcuda

%% sudo apt install libcudart11.0 %%

sudo apt install nvidia-cuda-toolkit


sudo ln /usr/lib/x86_64-linux-gnu/libEGL.so.1 /usr/lib/x86_64-linux-gnu/libEGL.so
```