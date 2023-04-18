# dell-latitude-e6530-hackintosh-big-sur
A prebuilt Opencore EFI for macOS Big Sur on the Dell Latitude E6530

This is a macOS Big Sur EFI for the Dell Latitude E6530, with support for Intel Wi-Fi cards. 11.7.6 working, with OpenCore 0.9.1 and fully up to date kexts. Remember to keep your kexts and OpenCore up to date! I recommend OCAuxiliaryTools to keep your kexts and OpenCore up to date. Remember to change your SMBIOS data too. 

![Screenshot](https://github.com/Lost-Entrepreneur439/dell-latitude-e6530-hackintosh-big-sur/blob/main/Screen%20Shot%202023-03-28%20at%209.48.30%20PM.png)

# Specs of my specific unit:
* CPU: Intel Core i5-3320m @ 2.6GHz
* GPU: Intel HD Graphics 4000
* RAM: 2x4GB Samsung 1333MHz DDR3
* Laptop model: Dell Latitude E6530
* Audio Codec: IDT92HD93BXX
* Ethernet card: I don’t remember the model but it was some type of Intel card
* Wi-Fi card: Intel Centrino Advanced-N 6205
* Touchpad: Alps
* BIOS: A22

Follow the "Downloading macOS" section in the Dortania guide to get macOS - https://dortania.github.io/OpenCore-Install-Guide/installer-guide/windows-install.html#downloading-macos

# Set BIOS settings as follows
* General -> Boot Sequence -> UEFI
* General -> Advanced Boot Options -> uncheck “Enable Legacy Option ROMs”
* System Configuration -> Parallel Port -> Disabled
* System Configuration -> Serial Port -> Disabled
* System Configuration -> SATA Operation -> AHCI
* Security -> TPM Security -> Uncheck “TPM Security”
* Secure Boot -> Secure Boot Enable -> Disabled
* Performance -> HyperThread control -> Enabled
* Power Management -> USB Wake Support -> Uncheck “Enable USB Wake Support”
* Power Management -> Wake on LAN/WLAN -> Disabled
* Virtualization Support -> Virtualization -> Check “Enable Intel Virtualization Technology”
* Virtualization Support -> VT for Direct I/O -> Uncheck “Enable VT for Direct I/O”

# Credits

* [Baggette](https://github.com/Baggette) for providing me his EFI and letting me use some parts from his EFI in mine.
* [Hervé](https://osxlatitude.com/profile/4953-herv%C3%A9/) for helping me fix graphical glitches and the SD card slot.
* [Jake Lo](https://osxlatitude.com/profile/1549-jake-lo/) for helping me fix sleep
* [Acidanthera](https://github.com/acidanthera)for making OpenCore, AppleALC, BrightnessKeys, IntelMausi, Lilu, RestrictEvents, VirtualSMC, VoodooPS2 and WhateverGreen
* [Dortania](https://github.com/dortania) for making CtlnaAHCIPort and the OpenCore Install Guide which was used to make this EFI
* [OpenIntelWireless](https://github.com/OpenIntelWireless/) for making Airportitlwm
* [1Revenger1](https://github.com/1Revenger1) for making ECEnabler
* [Sniki](https://github.com/Sniki) for making USBInjectAll
* [corpnewt](https://github.com/corpnewt) for making USBMap and SSDTTime
* [VoodooI2C](https://github.com/VoodooI2C) for making VoodooI2C and VoodooI2CHID
* [Apple](https://www.apple.com/) for making macOS.
* [Dell](https://www.dell.com/en-ca) for making the Latitude E6530