# Jetson-orin-nano-5.1.3

## Install pip
```
sudo apt update
```
```
sudo apt install python3-pip
```
```
sudo reboot
```

## Install Jtop
```
sudo pip3 install -U jetson-stats
```
```
sudo systemctl restart jtop.service
```
```
sudo reboot
```
After reboot
```
jtop
```

## Install VS Code

```
cd ~/Downloads
```
```
wget "https://code.visualstudio.com/docs/?dv=linuxarm64_deb"
```
sudo dpkg -i package_name.deb
```
```
sudo reboot
```

