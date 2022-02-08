---
layout: default
title: FAQ
description: Question asked | Answer given
light_mode: false
---

# 1. How do I control the fan speed on a Argon One case?
> 1. Enter the terminal by pressing F4 on the keyboard or access it via SSH.
> 2. enter ` curl https://download.argon40.com/argon1.sh | bash `
> 3. Customize fan speeds via ` argonone-config `
> 4. Uninstall with ` argonone-uninstall `

# 2. Where do I find config files etc.?
> [Files and Locations](guides/retropie/locations.md)

# 3. My Controller does not work via bluetooth. What can I do?
> _Answered by @MPoxon_
> Reinstall bluez
> 1. ` sudo apt --autoremove purge bluez `
> 2. ` sudo apt install bluez `

# 4. A game asked me to change the disk. How do I accomplish this?
> When a game asks for it, you can change the current disk in the RetroArch Disc Control menu:
> 1. Eject the current disk with Eject Disc
> 2. Select the right disk index with Current Disc Index
> 3. Insert the new disk with Insert Disc
> The above is for games which don't allow multi disk drive support.

# 5. How to disable specific overlays manually?
> To disable a specific overlay the manual way, Atari 2600 will be used as an example.
> 1. ` nano opt/retropie/configs/atari2600/retroarch.cfg `
> 2. comment the following line:   
> ` input_overlay = "/opt/retropie/emulators/retroarch/overlays/RickDangerous/exodus_cl-speakersonly.cfg" `   
> by inserting a hash:   
> ` #input_overlay = "/opt/retropie/emulators/retroarch/overlays/RickDangerous/exodus_cl-speakersonly.cfg" `

# 6. How to enable a different overlay for a specific system?
> Atari 2600 will be used as an example again to expain how to use a different overlay for a system.
> From above it is seen that the current overlay is exodus_cl-speakersonly
> It can be changed to a new overlay for example generic_atari2600_border
> 1. disable the previous overlay
> 2. enter ` input_overlay = "/opt/retropie/emulators/retroarch/overlays/RickDangerous/generic_atari2600_border.cfg" `
> 3. move the config file ` generic_atari2600_border.cfg `   
> aswell as the overlay file ` generic_atari2600_border.png `   
> to ` /opt/retropie/emulators/retroarch/overlays/RickDangerous/ `
> 4. if the downloaded overlay does not have a .cfg file it easily can be created   
> or another one can be copied and renamed to generic_atari2600_border.cfg
>
>     4.1 To create a new one open your favourite text editor (e.g. "notepad++" or in terminal "nano")
>
>     4.2 Enter:   
>     ` overlays = 1 `   
>     ` overlay0_overlay = generic_atari2600_border.png `   
>     ` overlay0_full_screen = true `   
>     ` overlay0_descs = 0 `
>
>     4.3 save as generic_atari2600_border.cfg (in this example)
>
> This can be done using the EmulationStation configuration editor in the options menu
> 1. Configure basic libretro emulator options
> 2. Configure additional options for example Atari 2600 overlay set to false to disable or true to enable

# 7. EmulationStation crashed upon first startup.
> Wrong HDMI port: The Raspberry Pi 4 has two HDMI ports. The connector on the left marked 'HDMI0' is the primary/default display. If you're using just 1 screen you'll need to use this one.
> If there is no display on startup with either hdmi:
> With some models of TV you may have to undertake a bit of 'trial and error' with the config.txt video settings. 
> There's a great Raspberry Pi article here detailing these settings on [raspberrypi.org](https://www.raspberrypi.org/documentation/configuration/config-txt/video.md)
> Changing hdmi_safe to 1 is a good first step, then go from there.

# 8. My Raspberry Pi won't connect to WiFi.
> Set your timezone/location   
> When you first set up a Raspberry Pi, sometimes you'll need to manually set the timezone/location to allow you to make a WiFi connection (even though the initial setup screens appear to set this for you). 
> 1. In a terminal window type in ` sudo raspi-config `, 
> 2. then ` Localisation Options ` 
> 3. then set your locale, timezone and WLAN country.
> See also [ThePiHut Support](https://support.thepihut.com/hc/en-us/articles/360014695877-Raspberry-Pi-won-t-connect-to-WiFi)

# 9. What hardware do you use?
> [RickDangerous' Setup](hardware/ricks_setup.md)

# 10. Exit from PSP or Dreamcast does not work.
> _Answered by @kerrz_
> Dreamcast:
> 1. Connect a keyboard.
> 2. Start a Dreamcast game
> 3. Hit ESC on your keyboard to Redream menu. 
> 4. Use W, A, S and D to navigate and L to select options (or use your controller). 
> 5. Go to INPUT > Port A/ Controller 0 > Main menu (if pushed by mistake you can resume) or Exit Emulator to get directly back to EmulationStation.
> 6. Choose the button to your liking. I chose the "Select" button for this, as it is not in use.   
> Pushing "select" inside a game will now get the main menu up, and you can exit from there.
> 
> PSP:
> 1. Connect a keyboard.
> 2. Start a PSP game
> 3. Hit ESC on your keyboard to PPSSPP menu. 
> 4. Use Arrow keys to navigate and Enter to select options (or use your controller). 
> 5. Go to SETTINGS > Controls > Control mapping.
> 6. Scroll down to "Pause", press "+" and choose the button to your liking that you want to use for exiting to the emulator.    
> Check that the button you choose is not used for other things. 

# 11. How do I use EmulationStation Hotkeys?
> [Hotkeys](guides/emulationstation/hotkeys.md)

# 12. My controller is not working.
> _Answered by @Rafamate_
> If you need to setup controllers from scratch and cannot use controller(s); using a keyboard you can go to:
> 1. RetroPie
> 2. RetroPie Setup 
> 3. Manage Configurations
> 4. EmulationStation
> 5. Clear input Configuration

# 13. How do I add a game to a collection?
> _Answered by @Rafamate_
> In EmulationStation, enter the Collection you want to add (or remove) games to. Press select and choose "add games to this collection", you can then navigate around different systems and add games by pressing Y button.
> Once you're happy with the games you've added, make sure you press Select again and choose "Finish editing collection", in order to save it.
> Be sure to shutdown properly or restart emulationstation to ensure it is kept next time you start your retropie!

# 14. How do I change the emulator if the game is not performing well?
> 1. When loading the game press X or A on your controller. 
> 2. Goto select ROM for the emulator (make sure just ROM).
> 3. Try lr-nestopia (if nes game) or another emulator.
> 4. Start the game and see if it performs better.
> 
> If you can't access that menu when booting a game it means run command is disabled. 
> 1. Options 
> 2. runcommand 
> 3. configuration 
> 4. make sure launch menu is set to enabled.

# 15. How do I update my pi so it can boot from usb?
> The simple short answer is: when in emulationstation, press F4 and write the following lines:
> 1. check if an update exist:   
> ` sudo rpi-eeprom-update `
> 2. if update exist, type in these two lines to install the update:   
> ` sudo rpi-eeprom-update -a `   
> ` sudo reboot `
> More info about eeprom on [raspberrypi.org](https://www.raspberrypi.org/documentation/computers/raspberry-pi.html#raspberry-pi-4-boot-eeprom)
> Initially, the pi will try to boot from the sd card. If nothing there, it will check if there is anything connected via usb that can boot up. So, if you do not change any boot config, your pi will boot from ssd if sd slot is empty, and when sd card is inserted, the pi will boot from there.

# 16. What software do you use to scrape new games?
> I use [Skraper](http://skraper.net/)

# 17. What software do you use to transfer new games?
> I use [WinSCP](https://winscp.net/eng/index.php)

# 18. How do I log into root user via cyberpunk or transmit on mac?
> _Answered by @QUIZASERAQ_
> There is no root password set by default so root login via cyberpunk or transmit on mac is not possible. 
> There are tutorials on how to set one but u should backup before.
> Quick steps:
> SFTP logging into RetroPie (with terminal or TRANSIT on a Mac)
> Log in (via remote terminal or on PI iteslf):
> 1. open Terminal Session    
> type: ssh pi@yo.ur.i.p   
> type: raspberry
> Now change root password
> 2. type: sudo nano /etc/ssh/sshd_config
> 3. change:   
> '#PermitRootLogin prohibit-password' to 'PermitRootLogin yes'
> 4. type: sudo passwd root
> 5. type in your new root password 
> 6. retype it
> 7. type: reboot
> Now you can log in to your pi as root with Transit, using the new password.
> Please always stop quit ES (by pressing F4 on connected keyboard | typing 'kill $(pidof emulationstation)' in  remote terminal) before altering any files or uploading new roms and media/gamelists!!! otherwise your existing gamelists may be corrupted!!!

# 19. How do I enable REWIND?
> _Answered by @kerrz_
> To enable REWIND in most games (Hotkey + L trigger):
> OPTIONS > Retroarch (steps 1-2-3 below start on main menu):
> 1. Settings > Inputs > Hotkeys
>
>     a. Rewind - set to L trigger button (L shoulder is occupied for load state).
>     b. Enable hotkeys - set to your hotkey ("select")
>     
> 2. Settings > Frame Throttle > Rewind > Rewind Support
>
>     a. Change the Buffer Size (MB) to around 100.
>
> 3. Configuration File > Save Current Configuration
> If you are not sure how trigger and shoulder buttons was defined, you can do it again; from the main theme, press Start and choose Configure Input.

# 20. How to check if my image is corrupt (Find MD5 checksum)?
> 1. open Windows Powershell 
> 2. go to the folder where your image file is present
> 3. in that folder, write: "Get-FileHash filename.img -Algorithm MD5"
> 4. Wait. This will take a lot of time. When finished, a number will show, which is the MD5 checksum.
> Or you can find the MD5 checksum (and others) of your image file utilizing Hashtab [implbits](http://implbits.com/) - thanks to _@share-and-enjoy_. 
> If the link above does not work, try this: [cnet](https://download.cnet.com/HashTab/3000-2094_4-84837.html)
> When Hashtab is installed, you go to the image file in windows explorer, right click it >> Properties >> Hash tab. 
> Depending on the size of the file and your computer, it will take some time to calculate the MD5 and SHA1. 

# 21. How do I boot from an SSD?
> [Boot from USB](guides/beginning/boot.md)

# 22. Where do I find my save files?
> _Answered by @kerrz_
> Save files are located in:
> ` home/pi/RetroPie/saves/<system> `

# 23. Can you recommend a torrent client?
> _Answered by @kerrz_
> Tixati or qbittorrent

# 24. How are the systems sorted?
> 0. Options
> 1. Arcade type systems by alphabet 
> 2. Consoles and handhelds type systems by manufacture - alphabetical order (Nintendo, Sega...)
>
>     2.1 Within each manufacture; by year
> 3. Computers by alphabet
> 4. Genres by alphabet
