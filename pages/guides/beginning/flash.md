---
layout: home
title: How To Flash
description: Disk Images
light_mode: false
---

# How to flash a disk image
_by @RickDangerous and @AzureOrange_

This guide shows you how to flash a disk image (like the ones RickDangerous built) onto a suitable drive.

## Recommended Software

Using **Windows** or **MacOS** you may use either [balenaEtcher](https://www.balena.io/etcher/) or the [Raspberry Pi Imager](https://www.raspberrypi.com/software/).

@RickDangerous personally uses balenaEtcher, so this option is confirmed to be working with his images. 

Using **Linux** you theoretically do not need an additional program to flash an image to a drive. You may simply use the dd command inside your favourite terminal.

## How to flash the image using balenaEtcher

1. Start the software
2. Select "flash from file"
3. Locate the image your going to flash
4. Select your target, which is the drive you're going to flash the image to.  
Be careful to double and tripple check, you're selecting the correct drive. Choosing a wrong one will destroy all data on it.
5. Then press flash!

If you have any problems flashing the drive using etcher, alternatively you can use the Raspberry Pi Imager.

## How to flash the image using the Raspberry Pi Imager

1. Start the Raspberry Pi Imager
2. Choose your operating system from the list or add the custom one
3. Choose your storage drive you want to flash onto.  
Be careful to double and tripple check, you're selecting the correct drive. Choosing a wrong one will destroy all data on it.
4. Click "write" 

## How to flash the image using your linux terminal

1. Open your terminal of choice
2. Enter the following command   
```
sudo dd if=/PATH/to/RickDangerous.img of=/dev/sdX bs=4M conf=fsync
```
where "if" points to the disk image and "of" to the disk you want to flash to (This might be /dev/sda, /dev/sdb etc.).  
Again be careful to double and tripple check, you're selecting the correct drive. Choosing a wrong one will destroy all data on it.

3. Hit enter and wait for the process to finish.

## How to flash the disk image using the Argon one case

[Flash using the Argon One case](flash_argon_one.md)
