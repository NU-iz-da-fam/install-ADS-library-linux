# install_ads_library_linux
## Introduction
- ADS or Automation Device Specification is a communication protocol developed by Beckhoff Automation, a company specializing in automation and control systems.
- ADS is prefered using in industrial field with real-time advantages.
## How to install

- 1. Clone the library from Beckhoff/ADS github
```bash
git clone https://github.com/Beckhoff/ADS.git
```
- 2. Create build folder and go in there
```bash
cd ADS/
mkdir build && cd build
```
- 3. Make, build and install.
```bash
cmake ..
cmake --build .
cmake --install .
```

## Warning
Sometimes, we will face the error that: "install TARGETS given target "ads" which does not exist in this directory". But don't mind, let's check your cmake version
and see if its version >= 3.13.0. If your version is lower, pls update. Check the link below for more information.
https://stackoverflow.com/questions/34443128/cmake-install-targets-in-subdirectories
