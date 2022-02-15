---
layout: retropie
title: How To RetroPie
description: Multiplayer using Netplay
light_mode: false
---

# How to play in Multiplayer
_by @AzureOrange_

The Netplay asset is pre-installed to RetroPie, so with any instance of RetroPie it may be launched and used.

## Prerequisites

1. Both parties must run the same version of RetroArch.
2. Both parties must run the same emulator.
3. Both parties must run the same rom.

## Host Player
One player must host the session. This one has to provide network details with the others for them to join.

### Netplay Setup

1. Inside the RetroPie configuration menu (Options) open "RetroArch Net Play"
2. Choose "Set mode, (H)ost or (C)lient" and set it to Host
3. Note you External IP and your Port
4. Make shure the selected Port is opened on your Router for both UDP and TCP
5. Choose a Netplay nickname
6. Hit OK on "Save Configuration"

### Start Game as Host

1. Press Hotkey+X to enter the RGUI Menu
2. Press B to go back
3. Enter Netplay
4. Enter Host
5. Choose Start Netplay Host

## Client Player
The other players may join the session als clients.

### Netplay Setup

1. Inside the RetroPie configuration menu (Options) open "RetroArch Net Play"
2. Choose "Set mode, (H)ost or (C)lient" and set it to Client
3. Choose "Set Port" and enter the port provided by your host.
4. Choose "Set host IP address" and enter the IP provided by your host.
5. Choose a Netplay nickname
6. Hit OK on "Save Configuration"

### Start Game as Client

1. Press Hotkey+X to enter the RGUI Menu
2. Press B to go back
3. Enter Netplay
4. Enter Connect to Netplay Host
5. Enter the provided Network details
6. Hope for the best