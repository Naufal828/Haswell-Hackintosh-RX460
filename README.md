[![macOS version](https://img.shields.io/static/v1?label=MacOS-Monterey&message=12.3.1&color=blueviolet)](https://www.apple.com/id/macos/monterey-preview/) 
[![macOS version](https://img.shields.io/static/v1?label=MacOS-Monterey&message=12.4&color=blueviolet)](https://www.apple.com/id/macos/monterey-preview/) 
[![macOS version](https://img.shields.io/static/v1?label=MacOS-Ventura&message=13.0&color=orange)](https://www.apple.com/id/macos/monterey-preview/)
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.8.0-informational.svg)](https://github.com/acidanthera/OpenCorePkg)
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.8.1-informational.svg)](https://github.com/acidanthera/OpenCorePkg)
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.8.2-informational.svg)](https://github.com/acidanthera/OpenCorePkg)
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.8.3-informational.svg)](https://github.com/acidanthera/OpenCorePkg)

<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/ProductPageIcon_1024x1024x32.png" width="150"/>

# Hackintosh Haswell Dekstop
##### Download EFI: [Releases](https://github.com/Naufal828/Haswell-Hackintosh-RX460/releases)

# IMPORTANT NOTES!!
- Before you use this efi, configure smbios on config.plist
and make sure you have your bios settings.
- This EFI Tested on monterey 12.3.1, 12.4, 12.6.7 work perfectly.
- and for those of you who use an amd gpu, to stream netflix via safari use smbios without an igpu, like imacpro 1.1 or macpro 7.1
- for asus b85m-g motherboard users who want front panel headphones to [work use alcid 11](https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/headphones.png) 

# Read For Setting your smbios
- [Platfrom Info ](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#platforminfo)
- [Bios Settings](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#intel-bios-settings)
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
- [Monterey Supported Smbios](https://dortania.github.io/OpenCore-Install-Guide/extras/monterey.html#supported-smbios)
- [Mac OS Installer](https://t.me/HackintoshLover/563870)


## Supported SMBIOS
| Type                 |            Comment                |
|----------------------|-----------------------------------|
| iMac17,1             | Haswell desktops with dGPU        |
| iMac16,2             | Haswell desktops with only an iGPU|

## Bios Settings
| Settins              |            Comment                |
|----------------------|-----------------------------------|
| Fast Boot            | Disable                           |
| Secure Boot          | Disable                           |
| Serial/COM Port      | Disable                           |
| Parallel Port        | Disable                           |
| SVT-d                | Disable                           |
| Thunderbolt          | Disable                           |
| Intel SGX            | Disable                           |
| Intel Platform Trust | Disable                           |
| CFG Lock             | Disable                           |
| VT-x                 | Enable                            |
| Above 4G decoding    | Enable                            |
| Hyper-Threading      | Enable                            |
| Execute Disable Bit  | Enable                            |
| OS type:             | Other UEFI Mode                   |
| DVMT Pre-Allocated   | 64Mb                              |
| SATA Mode            | AHCI.                             |


## Hardware

| Type                 | Name                              |
|----------------------|-----------------------------------|
| CPU                  | [Intel® Core™ i7-4790](https://ark.intel.com/content/www/id/id/ark/products/80806/intel-core-i74790-processor-8m-cache-up-to-4-00-ghz.html)             |
| Motherboard          | [Asus B85M-G](https://www.asus.com/Motherboards-Components/Motherboards/Business/B85MG/)                       |
| Audio                | Realtek® Audio Codec ALC887       |
| IGPU                 | Intel® HD Graphics 4600           |
| DGPU                 | [AMD Radeon RX 460 2GB](https://www.gigabyte.com/Graphics-Card/GV-RX460WF2OC-2GD#kf)         |
| Display              | [Koorui 27N1](https://koorui.net/products/27n1-koorui-27-inch-fhd-monitor-computer-monitor-ips-panel-1080p-75hz-hdmi-vga-99-srgb-5ms-response-eye-care-virtually-borderless-design-display-monitor)                          |
| RAM                  | 8GB DDR3 1600Mhz                  |
| Ethernet             | Realtek® 8111G Gigabit Lan        |
| Wi-Fi Bluetooth      | none                              |
| Storage              | Maxell SSD 120Gb Sata Interface   |
| Hardisk              | Seagate 500Gb , Samsung 320Gb     |
## Patches & Kexts
 - [[Kext] VirtualSMC](https://github.com/acidanthera/VirtualSMC)
 - [[Kext] Lilu](https://github.com/acidanthera/Lilu)
 - [[Kext] WhateverGreen](https://github.com/acidanthera/WhateverGreen)
 - [[Kext] AppleALC](https://github.com/acidanthera/AppleALC/)
 - [[Kext] RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X/releases)

## Functional

-  QE/CI of AMD Radeon RX460 2GB
-  Restart, Sleep and Shutdown
-  CPU Power Management
-  iMessage / FaceTime / iCloud / AppleTV /
-  Ethernet
-  HDMI Out
-  All Port USB
-  VDA Decoder Fully Support 
-  stream netflix / prime video / disney+.  via safari *using imac pro 1,1 smbios

## Doesn't Work
- Wifi
- Bluetooth
- AirDrop
- etc....

## Untested
- none

 
## Article
- https://dortania.github.io/OpenCore-Install-Guide/
- https://dortania.github.io/GPU-Buyers-Guide/
- https://dortania.github.io/OpenCore-Post-Install/universal/drm.html#fixing-drm


## Resource
- https://github.com/acidanthera/OpenCorePkg
- https://github.com/headkaze/Hackintool
- https://mackie100projects.altervista.org/opencore-configurator/
- https://github.com/corpnewt/ProperTree

## Benchmark Result
- [GeekBench 4 CPU Score](https://browser.geekbench.com/v4/cpu/16562352)
- [GeekBench 5 CPU Score](https://browser.geekbench.com/v5/cpu/15233933)
- [GeekBench 6 CPU Score](https://browser.geekbench.com/v6/cpu/1854724)
- [Metal Score](https://browser.geekbench.com/v5/compute/4910778)
- [OpenCL Score](https://browser.geekbench.com/v5/compute/4910786)

## Contact
 - [Contact Us](https://t.me/naufaliosk)

## Support Me
 - [For Buy a coffee](https://saweria.co/Naufaal)

## Special Thanks to
- [God](https://id.wikipedia.org/wiki/Tuhan)
- [Apple](https://www.apple.com) For MacOS
- [Acidantera](https://github.com/acidanthera) The maker of OpenCore
- [Dortania People](https://github.com/orgs/dortania/people) for the OpenCore Install Guide
- [Admin and all member group H4CK1NTOSH L0V3R](https://t.me/HackintoshLover) the best group evvawhh

## Screenshot
Screen Shot 2023-07-21 at 2.11.55 PM.png

<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screen%20Shot%202023-07-20%20at%203.38.24%20PM.png" width="500"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screen Shot 2023-07-21 at 2.11.55 PM.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/HOME.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screenshot 2022-07-06 at 1.04.59 PM.png" width="500"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/ABOUT.png" width="500"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/sensei.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/VIDEOPROC.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/PTXtmYcmLKlX88QM_480.jpg" width="500"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screenshot 2022-07-06 at 1.02.20 PM.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/CB15.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/cinebench%20r23.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/BLACKMAGIC%208K.png" width="1000"/>



