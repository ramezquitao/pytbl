# Python interface for the Tiny Pic Bootloader #

The pytbl.py is an application developed in  Python, used to upload HEX files to a  PIC microcontroller using the  Tiny Pic Bootloader firmware.

## Description ##

This software allows you to upload Intel.hex files to PIC microcontrolers programmed with the Tiny Pic BootLoader . It is written in Python, and uses the Python-Serial module.

The program can be used as a console application, or if you have installed the wxPython module, you can use a wxWidgets GUI.

This program was written to allow the Tiny Pic BootLoader to be used in a Linux environment. It should work in any platform supporting Python and Python-Serial.

Use this program at your own risk.

If you are successful using this software, please let me know.
Usage

```
pytbl.py [options] [-f FILENAME [-p PORT] [-b BAUDRATE]]
```

| --version 	| show program's version number and exit |
|:-----------|:---------------------------------------|
|  -h, --help 	| show the help message and exit |
|  -f FILENAME,--file=FILENAME |	Intel Hex formated file to be bootloaded. It is a required parameter when PORT or BAUDRATE are given. |
|  -p PORT, --port=PORT |	Integer number used to specify the serial port to be used. Ports are enumerated from 0. Default PORT=0 |
|  | -p 0 Linux /dev/ttyS0 - Windows COM1 |
|  | -p 1 Linux /dev/ttyS1 -Windows COM2 |
|  | -b BAUD, --baud=BAUD 	Baud rate to be used during the communication. Default: BAUDRATE=115200|

## Download ##

The latest development source code can be accessed using Subversion. The following will fetch the latest sources:




  * Using username: ` svn checkout https://pytbl.googlecode.com/svn/trunk/ pytbl --username ... `

  * Anonimous copy: ` svn checkout http://pytbl.googlecode.com/svn/trunk/ pytbl `

## Install ##

python setup.py install

## Comments, Bugs, Suggestions ##

> ramezquitao@cihologramas.com
## News ##

Apr 14 2008

> A patch was submitted by B. Antoine, to allow the use of Python (2.5.x) and wxwidget (2.8.7). Before this patch you received this error message:

> DeprecationWarning: The wxPython compatibility package
> is no longer automatically generated or activly maintained. Please
> switch to the wx package as soon as possible."

> The svn version now works fine.

Sep 22 2010
> The cihologramas svn server crashed, so this new repository was created using the last version of the pytbl.

## Todo ##

  * Test the program in other platforms.
  * Translate the comments to english
  * Clean up the code
  * Test it with other PICS (it has been tested only with the 16F877A, and the 18F452)
  * Complete the options as the original Windows software (blank memory, write configuration bits, etc)
  * ....

## Copyright ##

Copyright (C) 2005, 2006, 2007 Combustion Ingenieros Ltda.  http://www.cihologramas.com

Author: Ricardo Amezquita Orozco  ramezquitao@cihologramas.com

## License ##

This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.



[Return to ciprojects](http://code.google.com/p/ciprojects/)