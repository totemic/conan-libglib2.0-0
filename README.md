# conan-libglib2.0-0
Conan build files for packaging pre-built ubuntu library `libglib2.0-0` and `libglib2.0-dev` 

# Get download link from ubuntu 
x86:
```
sudo apt-get update
sudo apt-get download libglib2.0-dev --print-uris
sudo apt-get download libglib2.0-0 --print-uris
```

Arm:
```
sudo mv /etc/apt/sources.list /etc/apt/sources.list.old
echo "# deb [arch=amd64] http://archive.ubuntu.com/ubuntu/ xenial main multiverse restricted universe
deb [arch=armhf] http://ports.ubuntu.com/ubuntu-ports/ xenial main multiverse restricted universe
deb [arch=armhf] http://ports.ubuntu.com/ubuntu-ports/ xenial-updates main multiverse restricted universe
# deb [arch=amd64] http://archive.ubuntu.com/ubuntu/ xenial-updates main multiverse restricted universe
# deb [arch=amd64] http://security.ubuntu.com/ubuntu/ xenial-security main multiverse restricted universe
#http://ports.ubuntu.com/ubuntu-ports xenial/main armhf
" | sudo tee /etc/apt/sources.list


sudo apt-get update
apt-get download libglib2.0-dev:armhf --print-uris
apt-get download libglib2.0-0:armhf --print-uris
```
