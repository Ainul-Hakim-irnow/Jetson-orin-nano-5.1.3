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
1. Install pip
```
sudo apt install python3-pip
```

## Install Jtop
1. Install Jtop
```
pip install -U jetson-stats
```
2. Initialize service
```
sudo systemctl restart jtop.service
```
3. Reboot
```
sudo reboot
```
4. After reboot, check Jtop
```
jtop
```

## Install VS Code
1. You can download VS Code [here](https://code.visualstudio.com/docs/?dv=linuxarm64_deb)

2. Open terminal
```
cd ~/Downloads
```
3. Install VS Code *.deb file
```
sudo dpkg -i package_name.deb
```

## Install Pylon
1. You can download *.tar.gz file [here](https://drive.google.com/file/d/1AKmBRzHc4yT-R1AkfoSfUR2PYj0U7Uz_/view?usp=sharing)

2. Open terminal
```
cd ~/Downloads
```
3. Unzip the file
```
sudo tar -xvf pylon_package_name.tar.gz
```
4. Install dependencies
```
sudo apt-get install libxcb-cursor0
```
5. Install pylon software
```
sudo dpkg -i pylon_package_name.deb
```
6. Install codemeter runtime
```
sudo dpkg -i codemeter_package_name.deb
```
7. Setup USB
```
sudo /opt/pylon/share/pylon/setup-usb.sh
```
8. Check Pylon Software. If success install pypylon library
```
pip install pypylon
```
9. After successfull install pylon. Try it using [this](opencv.py) code above
