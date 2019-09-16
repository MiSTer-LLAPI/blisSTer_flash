# blisSTer firmware tool

## Installing
Copy blisSTer_flash to your Scripts folder on the root of the MiSTer SD card, script to make upgrading blisSTer firmware easy coming soon

## Building
- get the [Linaro Linux Target Binary Toolchain](https://linaro.org/downloads) for your platform, targeting arm-linux-gnueabihf, and make sure it is in your path. Make sure you have MSYS2 on Windows.
- Build [libusb](https://github.com/libusb/libusb/releases) with linaro toolchain, v1.0.23 is a known good release
- Build [libusb-compat](https://github.com/libusb/libusb-compat-0.1/releases) with linaro toolchain, v0.1.7 is a known good release
- build via: make CC=arm-linux-gnueabihf-gcc CXX=arm-linux-gnueabihf-g++ LD=arm-linux-gnueabihf-ld
