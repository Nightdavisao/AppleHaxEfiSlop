# Hackintoshing my poor Ideapad

* Model: Lenovo Ideapad 3 15ALC6, 82MF0004BR
* The current config.plist has been only tested with Sequoia (for my own dev needs), although it should work on Sonoma with a better compatibility.
* OpenCore version: I don't remember

There are some stuff that are intentionally excluded, like some kexts for the PS/2 keyboard and the I2C touchpad, but that's because I don't use this laptop as one would use conventionally.  
This is literally my desktop computer, the internal display no longer works and the hinges are somehow broken in a funny way. Not portable (*like an actual laptop should be*) at all.
The wi-fi driver being used is itlwm; I swapped the previous Realtek card it used to have with an AX210 card. However, since the Airport variant of itlwm still doesn't work under Sequoia (and Tahoe), wi-fi will only work if you use Heliport, and macOS sees the card as an Ethernet card instead. You'll need to use an Ethernet cable (or use the RNDIS kext and plug your Android device in RNDIS mode) to be able to install macOS.

I don't know this issue is specifically because the internal display of my laptop is detached, but after installing macOS, you'll need temporarily use WhateverGreen and remove NootedRed just get through the initial setup screen, since apparently the wizard window is off-screen.

Hackintosh is officially dead, by the way.
