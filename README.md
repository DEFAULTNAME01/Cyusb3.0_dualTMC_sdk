# Dual-Tianmouc Stereo Camera v2.0 based on 'Non-Global Shutter with Internal Clock Logic Trigger'  Frame Packaging Project SDK

This repository contains a C++ SDK (Host-side) for the Dual-Tianmouc Stereo Camera v2.0 system, which also covered the 'Tianmouc SDK miniomum version'.  
The system uses non-global shutter sensors equipped with internal clock logic triggering, and fpga provides frame packaging  & controls Cyusb phy chip functionality for data transmission and processing.

## Features

- Stereo (dual-lens) camera support
- Random Phase Frame Alignment(assembly) & packaging
- Efficient usb3.0 data transmission
- C++ SDK for host-side application development

## Description

This project is designed for Dual-Tianmouc Stereo Camera equipped with two TMc v1.0 sensors, has USB3.0 as the transmition port.  
It utilizes internal clock logic to trigger image acquisition and implements frame packaging technology for robust and efficient data handling on the host side.

# Acknowledgements to Pre-work Teams for the original implementation.
## Citation

This repository is forked from [original-author/original-repo](https://github.com/original-author/original-repo).
Please cite the original project if you use this code in your work.

># Tianmouc SDK miniomum version

>## usages

>### If you have the access to the source code of tianmouc-sdk full version

>1. install cyusb, opencv, lib-usb-1.0-dev
>2. cp libcyusb.so to ./lib
>3. run 'sh compile.sh'
>4. run the somple application for tianmouc-v1 by ./build/tianmoucv_app
>5. you can also use the ./build/libtianmouc.so for further development

>### If you dont have the access

>- only x86 supported because the shared .so files are compiled under x86, ubuntu24.04

>1. You can find another cmake file in ./lib, use it to replace the defualt one
>2. compile this project, you can still get the app


>## development log

>- init version 20241104
>-- bug: memory leak, cannot find where is the bug
>-- bug2: bad cone decoded result??
>-- bug3: cannot use disableSync api, repost "free( ) invalid xxx"
>-- bug4: very dirty stop
>- updated version 20240906
>- fixed all bugs
>- minimum develop kit
