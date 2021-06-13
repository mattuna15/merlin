# Merlin
## Learn how to create your own 32-bit system from scratch.

A flexible, open platform to learn or develop 32-bit hardware or software using either a physical or FPGA solution.

The project uses a modular design to allow you to extend or move in different directions should you so wish. At it's heart is the core of a Multicomp system from Grant Searle. http://searle.x10host.com/Multicomp/index.html

<hr>
<img width="1302" alt="Screenshot 2021-06-13 at 15 45 34" src="https://user-images.githubusercontent.com/16086727/121814582-bda0da80-cc69-11eb-8a86-3e689ef1d6d6.png">
<hr>

IDE: 
* New GCC version of EHBasic. Compiles using standard m68k toolchain. Requires Merlin Newlib and Bios.
* [Easy68K] (http://www.easy68k.com/moreinfo.htm)
* GCC M68K  (https://github.com/mattuna15/merlin-68k-toolchain)
  - Full working C/C++ environment (including Newlib) 
  - Assembler support with Vasm

<hr>

Hardware:

- FPGA: ARTY A7-35T https://store.digilentinc.com/arty-a7-artix-7-fpga-development-board/ (Required)
- GFX: Gameduino Dazzler Arduino shield https://excamera.com/sphinx/store.html#gameduino-3x-dazzler-for-arduino-39 (optional)
- Sound: OPL3 Duo https://www.tindie.com/products/cheerful/opl3-duo/ (or any OPL2/3 boards) (optional)
- RTC: https://store.digilentinc.com/pmod-rtcc-real-time-clock-calendar/ (or any mcp794xx RTC i2c) (optional)
- SD Card: https://store.digilentinc.com/pmod-microsd-microsd-card-slot/ (or any SPI sd card) (optional)
- Keyboard: https://store.digilentinc.com/pmod-ps2-keyboard-mouse-connector/ (or any PS2 interface card) (optional)

- Also requires 2nd usb-uart 3.3v cable/board to upload software.

<hr>

VHDL:

https://github.com/mattuna15/zed-68k/tree/arty-gd

<hr>

CPU:

* Framework Multicomp amended to 32bit addresses

* TG68 - 68000/020 CPU (heavily modified)

* VGA/HDMI - Gameduino 3X Dazzler

* Basic - EHBasic 68k (Now running within GCC)

* Board - ARTY A7-35T

* Sound - Twin OPL3 chips (FM) Gameduino PCM

<hr>

Storage:

* FAT32 SDHC Card support with C Fat Library
* UART interface with support for S-Record upload

<hr>

Software Examples & drivers:
* https://github.com/mattuna15/merlin-software

[Turbocharged Homebrew](https://www.facebook.com/groups/1609879555846636/)

[License](https://raw.githubusercontent.com/mattuna15/merlin/master/LICENSE)

<hr>
Project acknowledgments:<br>
https://github.com/kanpapa/mic68k<br>
https://github.com/ProfKelly/EASy68K<br>
https://github.com/TobiFlex/TG68K.C<br>
http://searle.x10host.com/Multicomp/index.html<br>
https://www.retrobrewcomputers.org/doku.php?id=boards:sbc:multicomp:papilio-duo:start<br>
https://github.com/MJoergen/dyoc<br>
https://github.com/jefftranter/68000<br>

<hr>
License:

“By downloading these files you must agree to the following: The original copyright owners of ROM contents are respectfully acknowledged. Use of the contents of any file within your own projects is permitted freely, but any publishing of material containing whole or part of any file distributed here, or derived from the work that I have done here will contain an acknowledgement back to myself, Grant Searle, and a link back to this page. Any file published or distributed that contains all or part of any file from this page must be made available free of charge.” - http://searle.x10host.com/Multicomp/index.html
