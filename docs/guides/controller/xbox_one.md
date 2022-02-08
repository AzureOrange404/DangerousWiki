---
layout: controller
title: How To Controller
description: XBox One Controller
light_mode: false
---

# How to pair and configure an XBox One Controller?
_by @AlfDeMelmac_

steps to add a xbox one controller. 
1. press the key function + f4 or only f4 (depend on keyboard)
2. write: sudo nano /opt/retropie/configs/all/autostart.sh
3. on the opened file write: sudo bash -c 'echo 1 > /sys/module/bluetooth/parameters/disable_ertm'
4. press ctrl. + x
5. choose 'y'
6. press enter
7. write: sudo reboot
8. go to options > bluetooth > enable bluetooth pair button on joystick > register and connect to bluetooth device (remove if was added previously) > select joystick and enter > DisplayYesNo > OK
9. assign buttons on emulation station configure joystick menu.
