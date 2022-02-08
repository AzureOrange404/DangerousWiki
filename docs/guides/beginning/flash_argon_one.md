---
layout: beginning
title: How To Flash
description: M.2 SSDs Using Argon One
light_mode: false
---

# Flashing an Image using Argon One with M.2 SSD
_by @RickDangerous_

If you are using the Argon One case with an M.2 SSD installed inside the case, then you
have a couple of options to connect the drive to the PC for flashing the image.

First option is using a USB A to USB A cable.
Plug one end of the calbe into the PC and the other end into the USB port on the expansion section
at the bottom of the case and flash the image to the drive.

Second option is to buy an enclosure for the M.2 SSD drive and flash the drive using the
enclosure, then remove the drive and install it into the Argon One case.

## Recommended Software to flash the image to the drive.

I personally use [balenaEtcher](https://www.balena.io/etcher/).

Using Etcher select flash from file, locate the image your going to flash and
then select target, which is the drive your going to flash it to. Then press flash!

If you have any problems flashing the drive using etcher, alternatively you can use
[Raspberry Pi Imager](https://www.raspberrypi.com/software/)

This is an example of a USB A male to male connector cable:

![usb_male.jpeg](../../../../assets/guides/usb_male.jpg "USB Type A Male to Male Connector")

This is an example of a M.2 to USB enclosure:

![m2_enclosure.jpeg](../../../../assets/guides/m2_enclosure.jpeg "M.2 SSD USB Enclosure")
