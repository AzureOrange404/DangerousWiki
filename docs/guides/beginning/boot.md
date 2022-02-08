---
layout: beginning
title: How To Display
description: Connection and Port Usage
light_mode: false
---

# How to boot from a USB Device?
_by @kerrz_

Change boot sequence on Raspberry Pi 4.
`Boot first USB, if no USB present, boot from SD card`

On your PC:
Insert an empty SD card (or one that is ok to be overwritten) and Open Raspberry Pi Imager.
1. Choose OS > Misc utility images > Bootloader > USB Boot
2. Storage > select your SD card (to be overwritten) 
3. Push write and let it complete writing and verify process.

On your Raspberry Pi 4:
1. Insert the newly created SD card into your Pi. Power on and Wait at least 10 seconds until the display becomes green, then power off the Raspberry Pi and remove the SD card.
2. Let the SSD boot with no card in SD slot first and let it finish booting.
3. Shut down.

You can now insert both your SSD and an SD card with an OS. 

The SSD (or whatever storage used via usb) will now boot first, even with an SD card inserted.    
If you remove the connected USB from the SSD, the SD card will boot.
