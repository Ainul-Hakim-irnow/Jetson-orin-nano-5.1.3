# Jetson-orin-nano-5.1.3
For Seeed Studio reComputer **DO NOT** use ```sudo apt upgarde```

## Table of Content
1. [Install Python 3.10 and enviroment(#Install-Python-3.10-and-enviroment)
2. [Install pip for python 3.10](#-Install pip for python 3.10)

## Install Python 3.10 and enviroment
1. Check if python 3.10 install
```
python3.10 --version
```
2. If no python 3.10 install;
```
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt install python3.10 python3.10-dev python3.10-venv
```
3. Check
```
python3.10 --version
```
4. Create environment
```
python3.10 -m venv vnev
```

## Install pip for python 3.10
```
sudo apt update
sudo apt install nano
```
1. Open bashrc
```
nano ~/.bashrc
```
2. Scroll to the bottom and paste;
```
alias pip='python3.10 -m pip'
```
3. Press ```Ctrl + X```, then ```Y``` to save, then ```Enter``` to exit
4. Apply change
```
source ~/.bashrc
```
5. Install pip
```
sudo apt install python3-pip
```
```
sudo python3.10 -m ensurepip --upgrade
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
