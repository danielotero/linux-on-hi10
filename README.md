### Introduction
This is my attempt to gather all the information in one place on how to support the [Chuwi Hi10 Pro](http://en.chuwi.com/product/items/Chuwi-Hi10-Pro.html) tablet on Linux.

The configuration will be around my distribution ([Arch Linux](https://www.archlinux.org/)), but I hope that all the instructions here can be easily adapted to other distributions. Be aware that Arch Linux it's a [rolling realese](https://en.wikipedia.org/wiki/Rolling_release) distribution, so all software used will be pretty recent.

### Basic hardware specifications
A more detailed review can be seen at [NotebookCheck](http://www.notebookcheck.net/Chuwi-Hi10-Pro-Tablet-Review.186738.0.html).

| Part         | Component                                |
| ------------ | ---------------------------------------- |
| Processor    | Intel® Atom™ x5-Z8350 CPU @ 1.44GHz      |
| Graphics     | Intel® HD Graphics 400                   |
| RAM          | DDR3 4096 MB @ 1066 MHz                  |
| Screen       | 10.1-inch IPS display @ 1920x1200 pixels |
| Connectivity | 802.11n and Bluetooth® 4.0               |
| Ports        | 1 USB Type-C™, 1 microUSB, 1 microHDMI®  |

### Current status
This table currently refers to the default Arch Linux kernel package version 4.16.2-1.

| Device                 | Status                    |
|------------------------|---------------------------|
| microSD card slot      | Yes                       |
| Internal flash storage | Yes                       |
| Graphics               | Yes                       |
| microUSB port          | Yes                       |
| Type-C USB port        | Not tested (charging works) |
| Incorporated USB hub   | Yes                       |
| Keyboard               | Yes                       |
| Touchpad               | Yes                       |
| 802.11n wireless       | Yes                       |
| Speakers               | No                        |
| Headphone plug         | Yes, with [plbossart/UCM](https://github.com/plbossart/UCM/tree/master/bytcr-rt5651) |
| Battery measurement    | Yes                       |
| Backlight control      | Yes                       |
| Power button           | Yes                       |
| Volume buttons         | Yes                       |
| Suspend                | Yes                       |
| Screen lid switch      | Yes                       |
| Touchscreen            | See [below](#touchscreen-configuration) |
| Accelerometer          | No                        |
| HDMI output            | Needs more testing        |
| HDMI audio output      | Not tested                |
| Bluetooth              | Not tested                |
| Active stylus pen      | Yes                       |
| Front camera           | No                        |
| Back camera            | No                        |
| Light Sensor           | Not tested                |

**Note:** This list is sorted by my own priorities.

### Touchscreen configuration
From linux 4.15 on, the `silead` in-tree kernel module should work, as long as you provide a valid firmware.

Try downloading [this file](https://github.com/onitake/gsl-firmware/raw/master/firmware/chuwi/hi10_pro-z8350/firmware.fw) to `/usr/lib/firmware/silead/mssl1680.fw`

Probably, the firmware needs heavy calibrations. Try using the [touchscreen/rotation](https://github.com/danielotero/linux-on-hi10/blob/master/touchscreen/rotation) script.
