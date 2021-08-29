# dictd-openrc
OpenRC Script for dictd

# Installation
### Arch Linux based distributions
1. Install the package from the [AUR](https://aur.archlinux.org/packages/dictd-openrc/)

### Non Arch Linux Based
1. Clone this repo
2. Install the file **dictd.init** in */etc/init.d/* with
```bash
install -m=755 -oroot dictd.init /etc/init.d/dictd
```

# Setup
After installing you should add the service to the system boot schedule with
```bash
sudo rc-update add dictd default
```

# How-to uninstall
### Arch Linux based distributions
1. Just remove it with pacman
```bash
pacman -Rs dictd-openrc
```

### Non Arch Linux Based
1. First remove it from the system startup
```bash
rc-update del dictd -a
```
2. Then just delete the script from your system
```bash
 rm /etc/init.d/dictd
```
