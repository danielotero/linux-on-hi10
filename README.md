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
| Touchscreen  | Silead GSL1680                           |
| Connectivity | Realtek 8723BS (802.11n & Bluetooth® 4)  |
| Accelerometer| Bosch BMC150                             |
| Light sensor | Capella CM3218                           |
| Camera (?)   | OmniVision OV2680                        |
| Ports        | 1 USB Type-C™, 1 microUSB, 1 microHDMI®  |

### Current status
This table currently refers to the default Arch Linux kernel package version 5.0.7-arch1

| Device                 | Status                    |
|------------------------|---------------------------|
| Internal flash storage | Yes                       |
| Graphics               | Yes                       |
| microUSB port          | Yes                       |
| Type-C USB port        | Yes                       |
| Incorporated USB hub   | Yes                       |
| Keyboard               | Yes                       |
| Touchpad               | Yes                       |
| 802.11n wireless       | Very badly                |
| Speakers               | Yes                       |
| Headphone plug         | Yes                       |
| Battery measurement    | Yes                       |
| Backlight control      | Yes                       |
| Power button           | Yes                       |
| Volume buttons         | Yes                       |
| Suspend                | Yes                       |
| Screen lid switch      | Yes                       |
| Touchscreen            | Yes (see [touchscreen](touchscreen) folder) |
| microSD card slot      | Sometimes, Unreliable     |
| Accelerometer          | Yes                       |
| HDMI output            | Yes                       |
| HDMI audio output      | No                        |
| Bluetooth              | Not tested                |
| Active stylus pen      | Yes                       |
| Front camera           | No                        |
| Back camera            | No                        |
| Light Sensor           | No                        |

**Note:** This list is sorted by my own priorities.

### To do
 - Check [this patch](https://lore.kernel.org/patchwork/patch/397958/) for the light sensor.
 - Search for ways to improve WiFi stability (BIOS?).
 - Investigate the touch screen home button.

### Notes
 Take also a look to the [willyneutron](https://github.com/willyneutron/lubuntu_in_chuwi_Hi10Pro) repo, which is more detailed!
