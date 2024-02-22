# i7 8700k Gigabyte Z370 Aorous 2.0 EFI Sonoma 14.3.1

This is the fully detailed guide on how to create a working Hackintosh machine using:

:small_blue_diamond: MacOS Sonoma 14.3.1 <br />
:small_blue_diamond: OpenCore 0.9.8 <br />
:small_blue_diamond: Processor: Intel Core i 7 8700k <br />
:small_blue_diamond: RAM: 32 GB 3200 Mhz <br />
:small_blue_diamond: Graphics: NVIDIA GTX 760 2GB DDR5 (Zotac Reference) <br />
:small_blue_diamond: SSD: ADATA 256 GB  <br />
:small_blue_diamond: SMBIOS: iMacPro 19.1 2019 <br />

This repository contains also EFI folder with all binaries produced meanwhile. The missing pieces might be however serial numbers or other hardware identifiers.

# Driver Working

:white_check_mark: MacOS Sonoma 14.3.1 <br />
:white_check_mark: Processor: Processor: Intel Core i 7 8700k :love_letter: <br />
:white_check_mark: Graphics: NVIDIA GTX 760 2GB DDR5 :warning: (should patch using geforce kepler)  <br /> 
:white_check_mark: Ehernet I225-V Added Without Kext just adding on boot args "dk.e1000=0" without quotes<br /> 
:white_check_mark: HDMI audio ( currently i'd use this,im use 3rd party focusrite 3rd ) <br />
:white_check_mark: All USB <br />
:white_check_mark: ThunderBolt <br />


# List Tools We Need

1. [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools) - Initial configuration
2. [Intel Power Gadget](https://github.com/trulyspinach/SMCAMDProcessor) - for monitoring amd ryzen
3. [Geforce Kepler Patcher](https://github.com/chris1111/Geforce-Kepler-patcher) - for patching nvidia kepler
4. [HackingTool by Headkaze](https://github.com/headkaze/Hackintool) - to verify settings on running macOS are fine; wasn't always working fine if `EFI` configuration had error on target machine


# Official Opencore

1. [OpenCore](https://dortania.github.io/OpenCore-Install-Guide/) - Opencore Official Website
