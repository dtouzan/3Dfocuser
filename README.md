# 3Dfocuser
3D focuser for indilib

## Draw
<img src="draw.png">

## Download
```sh
cd
git clone https://github.com/dtouzan/3Dfocuser

cd
mkdir -p ~/EAFpy
cp ~/3Dfocuser/Sources/*.py ~/EAFpy
```

## Install (For Raspberry Pi Zéro 2 W)
```sh
sudo cp ~/3Dfocuser/Build/indi_EAFpy_focuser /usr/bin/indi_EAFpy_focuser
sudo cp ~/3Dfocuser/Build/indi_EAFpy_focuser.xml /usr/share/indi/indi_EAFpy_focuser.xml
```

## Rebuild 

```sh
cd
mkdir build
cd build
cmake -DCMAKE_INSTALL_PREFIX=/usr -DCMAKE_BUILD_TYPE=Debug ~/3Dfocuser/Sources
make
sudo make install
```

## Start 
```sh
cd
indiserver indi_EAFpy_focuser indi_simulator_ccd
```

## Connect motor
<img src="connect_motor.png">

## Interface (With CCDCIEL)
### Connect
<img src="connect.png">

### Used
<img src="ticks.png">

### Driver info for speed
<img src="speed.png">

### Driver info for delay for step motor
<img src="delay.png">