Fine Offset Wireless Weather Station Reader

(C) 2010 Ane-Jørgen Auberg

Software is not released through any official channels, and thereby do not expect support from the vendor on this product.

This software is in no way affiliated or related to Fine Offset Electronics Co.,LTD. (http://www.foshk.com)

Product USB vendor details Vendor 1941, ID 8021

The application is written with inspiration from the following projects:
- WeatherStation.py - The pywws poject. http://pywws.googlecode.com
- usbsnoop2libusb.pl - The usbsnoop log file. The latest version of the script should be in http://iki.fi/lindi/usb/usbsnoop2libusb.pl
- wwsr.c - Wireless Weather Station Reader by Michael Pendec (michael.pendec@gmail.com)

Copyright (C) 2010 Arne-Jørgen Auberg  (arne.jorgen.auberg@gmail.com)

	This program is free software; you can redistribute it and/or modify
	it under the terms of the GNU General Public License as published by
	the Free Software Foundation; either version 2 of the License, or
	(at your option) any later version.
	
	This program is distributed in the hope that it will be useful,
	but WITHOUT ANY WARRANTY; without even the implied warranty of
	MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
	GNU General Public License for more details.
	
	You should have received a copy of the GNU General Public License along
	with this program; if not, write to the Free Software Foundation, Inc.,
	51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.

Dependencies:
- libusb (http://libusb.sf.net)
- json-c (http://www.github.com/json-c/json-c)

Brief introduction to functionality.
- The application is called through a script called by cron.
- All other parameters are shown when running the application either with the -h option, or without any arguments.

Current status:
- Reads all weather station data, not all data is decoded or used.
- Caching of previously read weather station values.
- No writing of data, this must be performed using  the EasyWeather application or the console display.
- Tested on OpenWrt, an embedded Linux distro
- Device gets claimed by the kernel usbhid driver, try running this program as root if you have problems to give it permissions to detach the attached drivers on startup.

TODO:
- More log formats
