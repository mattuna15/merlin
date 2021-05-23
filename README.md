# Merlin
## Learn how to create your own 32-bit system from scratch.

We aim to provide a flexible, open platform to learn or develop 32-bit hardware or software using either a physical or FPGA Arm-style solution.

The project will be built up in sections or episodes and use a modular design to allow you to extend or move in different directions should you so wish.

IDE: 
* [Easy68K] (http://www.easy68k.com/moreinfo.htm)
* GCC M68K  (https://github.com/mattuna15/merlin-68k-toolchain)
  - Full working C/C++ environment (including Newlib) 
  - Assembler support with Vasm
  
Hardware:

FPGA: ARTY A7-35T https://store.digilentinc.com/arty-a7-artix-7-fpga-development-board/ (Required)
GFX: Gameduino Dazzler Arduino shield https://excamera.com/sphinx/store.html#gameduino-3x-dazzler-for-arduino-39 (optional)
Sound: OPL3 Duo https://www.tindie.com/products/cheerful/opl3-duo/ (or any OPL2/3 boards) (optional)
RTC: https://store.digilentinc.com/pmod-rtcc-real-time-clock-calendar/ (or any mcp794xx RTC i2c) (optional)
SD Card: https://store.digilentinc.com/pmod-microsd-microsd-card-slot/ (or any SPI sd card) (optional)
Keyboard: https://store.digilentinc.com/pmod-ps2-keyboard-mouse-connector/ (or any PS2 interface card) (optional)

Also requires 2nd usb-uart 3.3v cable/board to upload software.


VHDL:

https://github.com/mattuna15/zed-68k/tree/arty-gd

CPU:

* Framework Multicomp amended to 32bit addresses

* TG68 - 68000/020 CPU (heavily modified)

* VGA/HDMI - Gameduino 3X Dazzler

* Basic - EHBasic 68k

* Board - ARTY A7-35T

* Sound - Twin OPL3 chips (FM) Gameduino PCM

Storage:

* FAT32 SDHC Card support with C Fat Library
* UART interface with support for S-Record upload

Software Examples & drivers:
* https://github.com/mattuna15/merlin-software



[Turbocharged Homebrew](https://www.facebook.com/groups/1609879555846636/)

[License](https://raw.githubusercontent.com/mattuna15/merlin/master/LICENSE)
