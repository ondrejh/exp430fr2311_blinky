exp430fr2311_blinky - compile and run ti example code with msp430_gcc
=====================================================================

Description:

Project shows howto simply compile and flash [MSP430FR231x_Code_Examples](http://www.ti.com/lit/zip/slac708) using [make](https://www.gnu.org/software/make/), [msp430_gcc](http://www.ti.com/tool/msp430-gcc-opensource) and [MSP430Flasher](http://www.ti.com/tool/msp430-flasher) tools.

How to use it:

1) On windows: Get and install MINGW or something with "make" command in it and add it into you PATH variable. [Git command line tool](https://git-scm.com/) can be used too. On linux you probably have the tool already (just type "make --version" from you command line to test it).

2) Install [msp430_gcc](http://www.ti.com/tool/msp430-gcc-opensource).

3) Install [MSP430Flasher](http://www.ti.com/tool/msp430-flasher).

4) Change your msp430_gcc path and MSP430Flasher path in the project Makefile.
Edit lines
'''GCC_DIR ?= C:/ti/msp430_gcc
FLASHER := C:/ti/MSPFlasher_1.3.10/MSP430Flasher'''
according to your instalation.

5) Run command line utility in the project directory. Type "make" to compile the code.

6) Connect you EXP430FR2311 launchpad and run "make program" to flash the binary into the device.

7) Change the code file *.c with whichever example from [MSP430FR231x_Code_Examples](http://www.ti.com/lit/zip/slac708), modifi it or write you own.