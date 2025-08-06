# Jetson-orin-nano-5.1.3
For Seeed Studio reComputer **DO NOT** use ```sudo apt upgarde```

## Install Python 3.10
1. Check if python 3.10 install
```
python3.10 --version
```
2. Check if default python version
```
python3 --version
```
3. If no python 3.10 install;
```
sudo apt install python3.10 python3.10-dev python3.10-venv
```
4. Check
```
python3.10 --version
```
5. Set python 3.10 as highest priority
```
sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.8 1
sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.9 2
sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.10 3
```
6. Update pyhton 3.10 as default
```
sudo update-alternatives --config python3
```
7. Check the default
```
python3 ---version
```

## Install pip
```
sudo apt update
```
Install pip
```
sudo apt install python3-pip
```
```
sudo reboot
```

## Install Jtop
```
sudo pip install -U jetson-stats
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
You can download VS Code [here](https://code.visualstudio.com/docs/?dv=linuxarm64_deb)

Open terminal
```
cd ~/Downloads
```
```
sudo dpkg -i package_name.deb
```

## Install Pylon
You can download *.tar.gz file [here](https://drive.google.com/file/d/1AKmBRzHc4yT-R1AkfoSfUR2PYj0U7Uz_/view?usp=sharing)

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
Check Pylon Software. If success install pypylon library
```
pip install pypylon
```
After successfull install pylon. Try it using [this](opencv.py) code above
