---
layout: terminal
title: How To Terminal
description: How to enter and use the Terminal
light_mode: false
---

# The RetroPie Terminal
_by @AzureOrange_

RetroPie is based on a Debian Linux distro, which actually does not provide a GUI (Graphical User Interface) and only consists of a bash terminal.
Anything graphical inside RetroPie is provided by EmulationStation and RetroArch.

## How to enter the Terminal?

To enter the RetroPie Terminal simply connect a keyboard to the Raspberry Pi and configure it inside EmulationStation as a controller.

After configuring press the F4 key on the keyboard and RetroPie will switch to terminal.

Using the terminal any Linux package may be installed and executed.

To execute a command as root user (which will be necessary when a command returns "Permission denied") you may use ```sudo``` before the command.

e.g. ```sudo nano file.txt``` 

## How to exit the Terminal?

To exit the terminal and return to EmulationStation the command ```exit``` may be run.

## Useful bash commands

This guide provides a list of bash commands, which will be useful when working with RetroPie.

[Useful Commands](commands.md)
