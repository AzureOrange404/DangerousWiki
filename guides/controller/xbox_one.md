---
layout: controller
title: How To Controller
description: XBox One Controller
light_mode: false
---

# How to pair and configure an XBox One Controller?
_by @AlfDeMelmac_

These are the steps to add an xbox one controller to RetroPie: 
1. Press the key function + f4 or only f4 (depending on keyboard)
2. Write: ` sudo nano /opt/retropie/configs/all/autostart.sh `
3. On the opened file write: ` sudo bash -c 'echo 1 > /sys/module/bluetooth/parameters/disable_ertm' `
4. Press ctrl. + x to exit nano
5. Choose 'y' for yes to save
6. Press enter
7. Write: ` sudo reboot `
8. Go to options > bluetooth > enable bluetooth pair button on joystick > register and connect to bluetooth device (remove if was added previously) > select joystick and enter > DisplayYesNo > OK
9. Assign buttons on emulation station configure input menu.
