# vagrant
vagrant for wsl

# setup
## windows
### install virtualbox
https://www.virtualbox.org/wiki/Downloads

## wsl
### install vagrant
https://developer.hashicorp.com/vagrant/downloads

### configure
```
vim ~/.bashrc
```
Modify windows_username
```
export VAGRANT_WSL_ENABLE_WINDOWS_ACCESS="1"
export VAGRANT_WSL_WINDOWS_ACCESS_USER=<windows_username>
export VAGRANT_WSL_WINDOWS_ACCESS_USER_HOME_PATH=/mnt/c/vagrant
export PATH="$PATH:/mnt/c/Windows/System32/"
export PATH="$PATH:/mnt/c/Windows/System32/WindowsPowerShell/v1.0"
export PATH="$PATH:/mnt/c/Program Files/Oracle/VirtualBox"
```
```
mkdir -p /mnt/c/vagrant
```
```
source ~/.bashrc
```