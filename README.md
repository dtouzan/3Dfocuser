# 3Dfocuser
3D focuser for indilib

# Draw

# install
```sh
sudo cp indi_EAFpy_focuser /usr/bin/indi_EAFpy_focuser
sudo cp indi_EAFpy_focuser.xml /usr/share/indi/indi_EAFpy_focuser.xml

mkdir -p ~/EAFpy
cp MoveInfo.py EAFpyGPIO_OUT.py EAFpyMotor.py ~/EAFpy
```


# Rebuild 

```sh
mkdir -p ~/indi-EAFpy-Focuser
cp CMakeLists.txt config.h.cmake indi_EAFpy_focuser.cpp indi_EAFpy_focuser.h indi_EAFpy_focuser.xml.cmake
mkdir build
cd build
cmake -DCMAKE_INSTALL_PREFIX=/usr -DCMAKE_BUILD_TYPE=Debug ~/indi-EAFpy-Focuser
make
sudo make install
```

