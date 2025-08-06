# Jetson-orin-nano-5.1.3
For Seeed Studio reComputer **DO NOT** use ```sudo apt upgarde```

## Install Python 3.10
Check if python 3.10 install
```
python3 --version
```
If no
```


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
Copy and paste this url to the browser
```
https://code.visualstudio.com/docs/?dv=linuxarm64_deb
```
Open terminal
```
cd ~/Downloads
```
```
sudo dpkg -i package_name.deb
```
```
sudo reboot
```

## Install Pylon
Copy and paste this url to the browser. Download *.tar.gz file
```
https://drive.google.com/file/d/1AKmBRzHc4yT-R1AkfoSfUR2PYj0U7Uz_/view?usp=sharing
```
Open terminal
```
cd ~/Downloads
```
```
sudo tar -xvf pylon_package_name.tar.gz
```
```
sudo apt-get install libxcb-cursor0
```
```
sudo dpkg -i pylon_package_name.deb
```
```
sudo dpkg -i codemeter_package_name.deb
```
```
sudo /opt/pylon/share/pylon/setup-usb.sh
```
