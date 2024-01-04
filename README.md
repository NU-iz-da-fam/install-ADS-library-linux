# Install Twincat ADS Library with Linux
## Introduction
- ADS or Automation Device Specification is a communication protocol developed by Beckhoff Automation, a company specializing in automation and control systems.
- ADS is prefered using in industrial field with real-time advantages.

## Requirements
- ```cmake version >= 3.13.0``` to avoid "install TARGETS given target "ads" which does not exist in this directory".
- Reference link: https://stackoverflow.com/questions/34443128/cmake-install-targets-in-subdirectories
## How to install

1. Clone the library from Beckhoff/ADS github
```bash
git clone https://github.com/Beckhoff/ADS.git
```
2. Create build folder and go in there
```bash
cd ADS/
mkdir build && cd build
```
3. Make, build and install.
```bash
cmake ..
cmake --build .
sudo cmake --install .
```

## Update CMake
- Sure that after updating cmake, your library will be installed properly.
- You can check the link below for reference how to update cmake. https://gist.github.com/bmegli/4049b7394f9cfa016c24ed67e5041930 .    
- Then, remember to install by
```
sudo make install
```
