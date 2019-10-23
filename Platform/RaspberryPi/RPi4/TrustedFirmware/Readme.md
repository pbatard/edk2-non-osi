ARM Trusted Firmware for Raspberry Pi 4
=======================================

The `bl1.bin` and `fip.bin` ATF binaries found in this directory are custom builds
produced from https://github.com/andreiw/lampone-tf-a and not the official ATF source.

For Raspberry Pi 4 usage, ATF was built using the command:
```
make PLAT=rpi4 PRELOADED_BL33_BASE=0x30000 RPI3_PRELOADED_DTB_BASE=0x10000 SUPPORT_VFP=1 RPI3_USE_UEFI_MAP=1 DEBUG=0 fip all
```
