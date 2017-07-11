### Introduction
This is my attempt to gather all the information in one place on how to support the [Chuwi Hi10 Pro](http://en.chuwi.com/product/items/Chuwi-Hi10-Pro.html) tablet on Linux.

The configuration will be around my distribution ([Arch Linux](https://www.archlinux.org/)), but I hope that all the instructions here can be easily adapted to other distributions. Be aware that Arch Linux it's a [rolling realese](https://en.wikipedia.org/wiki/Rolling_release) distribution, so all software used will be pretty recent.

### Basic specifications
A more detailed review can be seen at [NotebookCheck](http://www.notebookcheck.net/Chuwi-Hi10-Pro-Tablet-Review.186738.0.html).

| Part         | Component                                |
| ------------ | ---------------------------------------- |
| Processor    | Intel® Atom™ x5-Z8350 CPU @ 1.44GHz      |
| Graphics     | Intel® HD Graphics 400                   |
| RAM          | DDR3 4096 MB @ 1066 MHz                  |
| Screen       | 10.1-inch IPS display @ 1920x1200 pixels |
| Connectivity | 802.11n and Bluetooth® 4.0               |
| Ports        | 1 USB Type-C™, 1 microUSB, 1 microHDMI®  |

### What's working?

| Device                 | Status                    |
|------------------------|---------------------------|
| microSD card slot      | No                        |
| Internal flash storage | Yes                       |
| Graphics               | Yes                       |
| microUSB port          | Yes                       |
| Type-C USB port        | Only charging             |
| Incorporated USB hub   | Yes                       |
| Keyboard               | Yes                       |
| Touchpad               | Yes                       |
| 802.11n wireless       | Yes (4.12 staging driver) |
| Speakers               | No                        |
| Headphone plug         | No                        |
| Battery measurement    | Yes                       |
| Backlight control      | Yes, with [this](https://bugs.freedesktop.org/show_bug.cgi?id=85977#c38) tweak |
| Power button           | Yes                       |
| Volume buttons         | Yes                       |
| Suspend                | Yes? Needs more testing   |
| Screen lid switch      | Yes                       |
| Touchscreen            | With [gslx680-acpi](https://github.com/onitake/gslx680-acpi) |
| Accelerometer          | No                        |
| HDMI output            | Yes? Needs more testing   |
| HDMI audio output      | Not tested                |
| Bluetooth              | Not tested                |
| Active stylus pen      | Not tested                |
| Front camera           | No                        |
| Back camera            | No                        |
| Light Sensor           | Not tested                |

**Note:** This list is sorted by my own priorities.
