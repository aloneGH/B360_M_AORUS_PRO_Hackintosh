# B360_M_AORUS_PRO_Hackintosh
Hackintosh with OpenCore under B360 M Aorus Pro motherboard.

## Specs:

* `CPU`: Intel i3-8100
* `Motherboard`: GigaByte B360 M Aorus Pro
* `Memory`: Kingston DDR4 24000 32GB(8GBx4)
* `Storage`: WDC SN500 NVMe 500GB
* `Graphics`: Intel UHD Graphics 630
* `Monitor`: AOC Q2490PXQ 23.8 2K


## Working:

* CPU dynamic frequency
* Display with 2k resolution using DisplayPort
* Audio
* Ethernet
* USB(2.0 & 3.0)
* App store, iCloud, iMessage, iTunes, FaceTime, etc
* Sleep, Wakeup, Shutdown, Restart


## Not Working:

* Wifi and BT(not completed working)
* Airdrop, Hand-off


## Tutorial

* Model: iMac19,2
* MacOS Version: 10.14.6
* Bootloader Manager: `OpenCore 0.5.6`
* Installation Guide: [r/hackintosh](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)


## Notice

This motherboard can not disable CFG-Lock from BIOS settings, so there is something to do before installing. There are two options:

* [Fixing CFG-Lock](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/extras/msr-lock) (recommend)
* Enable the following from config.plist under `Kernel` -> `Quirks`: `AppleCpuPmCfgLock`, `AppleXcpmCfgLock`
