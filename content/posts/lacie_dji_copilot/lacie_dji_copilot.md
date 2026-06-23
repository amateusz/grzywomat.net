---
date: 2026-05-12T21:05:41+02:00
draft: false
title: "\"I found a weird, broken device\" (aka LaCie DJI Copilot)"
weight: 10
summary: Hard to love portable back-up station repair
description: Pretty modern device that is pretty hard to use in 2026
---

First let me introduce this device, as it's a dead product with not many mentions on the internet:

<div style="display: flex; gap: 10px;">
  <img style="height: 300px; width: auto; flex: 1 1 auto; object-fit: cover; background-color: white" src="../pictures/lacie-dji-copilot-external-drone-data-drive-2tb-side.png" />
  <img style="height: 300px; width: auto; flex: 1 1 auto; object-fit: cover; background-color: white" src="../pictures/lacie-dji-copilot-external-drone-data-drive-2tb-package.png" /> 
</div>

# LaCie DJI Copilot
It is a backup station for content creators made by LaCie and sold around 2018-2021. It was intended for drone fotage, but I don't see anything special about it besides "DJI" branding. It has a 2TB hard drive inside. 

It is not so easy to understand how to use it. I think it's a really cool device that they made, but challenging grasp how to use it.
It also has a sleep mode, which makes it more complicated.
I try to think of it as a linux computer with a attached storage and host/device ports.

## Modes
It has 3 different modes and it has many hardware ports. Each port is supposed to be used in a given way, otherwise it's "not tested/unsupported".

1.a. Stand-alone
In this mode you can back-up SD card and/or a USB storage onto the internal 2TB drive. It is a full copy, not incremental you can only start it and stop it.

1.b. Stand-alone with smartphone
Connecting a smartphone with an app ("LaCie DJI Copilot BOSS") to the microUSB host port allows for more interactive 1.a. You have now more control over back-ups, can manage files and settings. Also in this mode you can back-up your whole LaCie drive onto another 2TB USB disk.

2. Connected to a computer via USB device
In this mode a host computer gets an exclusive access to device's hard drive, SD card and USB a port. This mode makes this device still useful, even if battery and app dies – IN THEORY.

###
I found my copy not working and with just microUSB–iPhone cable.
The device was totally dead, albeit I didn't have a barrel jack power supply.
I disassembled it and started to poke around:
The hard drive is just a standard SATA 2.5" HDD.
The battery is a 2 cell (7.4V nom.) LiPol battery, and it has failed. One of the pouches was full of gas, so it's ESR is likely very high and it does not work.

I fashioned a replacement battery from my stock, but unfortunately it is quite bad as well, so the device browns-out when there is a phone charging off of it.

What I learned:
 - maximum dimensions for the battey are 6.5×66×106mm. Do not try to fit any bigger there. I tried and stopped while I could.
 - the app cannot be installed on iOS device in 2026
 - the app can be installed on a Android phone, I provide the APK found on the internet
 - custom proprietary cable for mode 1.b. is just a microUSB host cable (OTG), with device port on the other end (USB C, microUSB, Lightning)
 - it does charge through USB C (mode 2.) when the battery is fully dead
 - barrel jack connector is a×b TBD
 - when you connect a battery, the device needs to be revived, even if the battery is full by connecting 12V barrel jack

