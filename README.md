![macOS version](https://img.shields.io/static/v1?label=MacOS-Sonoma&message=14.0&color=green)
![OpenCore version](https://img.shields.io/badge/OpenCore-0.9.9-informational.svg)


<img src="https://cdn.jim-nielsen.com/macos/512/macos-sonoma-2023-09-26.png?rf=1024" width="150"/>


# Hackintosh Haswell Dekstop
##### Download EFI: [Releases](https://github.com/Naufal828/Haswell-Hackintosh-RX460/releases)

# IMPORTANT NOTES!!
- Before you use this efi, configure smbios on config.plist
and make sure you have your bios settings.
- This EFI Tested on monterey 12.3.1, 12.4, 12.6.7 work perfectly.
- and for those of you who use an amd gpu, to stream netflix via safari use smbios without an igpu, like imacpro 1.1 or macpro 7.1
- for asus b85m-g motherboard users who want front panel headphones to work use [alc id 11](https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/headphones.png)
- use of different motherboard, cpu or smbios may require re-mapping usb
- required amd gpu Polaris+ for gpu acceleration. because Intel HD 4600 is no longer supported for Mac OS Ventura or higher

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
| Motherboard          | [Asus B85M-G](https://www.asus.com/supportonly/b85m-g/helpdesk_cpu/)                       |
| Audio                | [Realtek® Audio Codec ALC887](https://semiconductors.es/datasheet/ALC887.html)       |
| IGPU                 | [Intel® HD Graphics 4600](https://www.techpowerup.com/gpu-specs/hd-graphics-4600.c1994)           |
| DGPU                 | [AMD Radeon RX 460 2GB](https://www.gigabyte.com/Graphics-Card/GV-RX460WF2OC-2GD#kf)         |
| Display              | [DELL SE2719H](https://www.amazon.com/Dell-backlit-Monitor-SE2719H-1080p/dp/B07KW6HFD1)                          |
| RAM                  | 16GB DDR3 1600Mhz                  |
| Ethernet             | Realtek® 8111G Gigabit Lan        |
| Wi-Fi Bluetooth      | [Intel AC 7265](https://www.tokopedia.com/zonabarang/intel-ac7265-ngw-high-speed-wifi-card-pcie-1x-dual-band-bluetooth)                            |
| Storage              | [Adata SU650 1TB](https://www.tokopedia.com/atkiosk/adata-ultimate-su650-1tb-ssd-sata-2-5-garansi-3-tahun?extParam=ivf%3Dfalse&src=topads)   |

## Patches & Kexts
 - [[Kext] VirtualSMC](https://github.com/acidanthera/VirtualSMC)
 - [[Kext] Lilu](https://github.com/acidanthera/Lilu)
 - [[Kext] WhateverGreen](https://github.com/acidanthera/WhateverGreen)
 - [[Kext] AppleALC](https://github.com/acidanthera/AppleALC/)
 - [[Kext] RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X/releases)
 - [[Kext] Itlwm](https://github.com/OpenIntelWireless/itlwm/releases)
 - [[Kext] IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)

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
-  Wifi
-  Bluetooth

## Doesn't Work
- airdrop
- screen mirroring from iphone

## Untested
- AirDrop not tested on Intel AC 7265 

 
## Article
- https://dortania.github.io/OpenCore-Install-Guide/
- https://dortania.github.io/GPU-Buyers-Guide/
- https://dortania.github.io/OpenCore-Post-Install/universal/drm.html#fixing-drm
- https://openintelwireless.github.io/itlwm/Installation.html
- https://openintelwireless.github.io/IntelBluetoothFirmware/Installation.html


## resources
- https://github.com/acidanthera/OpenCorePkg
- https://github.com/headkaze/Hackintool
- https://mackie100projects.altervista.org/opencore-configurator/
- https://github.com/corpnewt/ProperTree
- https://github.com/0xCUB3/About-This-Hack

## Benchmark CPU Result

| SINGLE CHANNEL 8GB            |           DUAL CHANNEL 16GB               |
|----------------------|-----------------------------------|
| [GeekBench 4 CPU Score](https://browser.geekbench.com/v4/cpu/16562352)           | [GeekBench 4 CPU Score](https://browser.geekbench.com/v4/cpu/17181025)                          |
| [GeekBench 5 CPU Score](https://browser.geekbench.com/v5/cpu/15233933)        | [GeekBench 5 CPU Score](https://browser.geekbench.com/v5/cpu/22156194)                          |
| [GeekBench 6 CPU Score](https://browser.geekbench.com/v6/cpu/1854724)    | [GeekBench 6 CPU Score](https://browser.geekbench.com/v6/cpu/4488959)                          |


## Benchmark GPU Result
| SINGLE CHANNEL 8GB            |           DUAL CHANNEL 16GB               |
|----------------------|-----------------------------------|
| [GeekBench METAL Score](https://browser.geekbench.com/v5/compute/4910778 )           | [GeekBench METAL Score](https://browser.geekbench.com/v5/compute/6709524 )                          |
| [GeekBench OPENCL Score](https://browser.geekbench.com/v5/compute/4910786)        | [GeekBench OPENCL Score](https://browser.geekbench.com/v5/compute/6709525 )                          |


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
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screenshot 2024-01-09 at 6.02.47 PM.png" width="500"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screenshot%202024-02-04%20at%207.41.14%20AM.png" width="500"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/headphones.png" width="500"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screen%20Shot%202024-01-17%20at%205.20.03%20AM.png" width="500"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screen%20Shot%202024-01-17%20at%205.20.07%20AM.png" width="500"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screenshot%202024-01-21%20at%205.11.08%20PM.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screenshot%202024-01-27%20at%2010.23.03%20AM.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screenshot%202024-01-27%20at%2010.23.13%20AM.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/HOME.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screen Shot 2023-07-21 at 2.11.55 PM.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screenshot%202024-01-28%20at%206.06.34%20PM.png" width="500"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/ABOUT.png" width="500"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/sensei.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/VIDEOPROC.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/PTXtmYcmLKlX88QM_480.jpg" width="500"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/Screenshot 2022-07-06 at 1.02.20 PM.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/CB15.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/cinebench%20r23.png" width="1000"/>
<img src="https://github.com/Naufal828/Haswell-Hackintosh-RX460/blob/main/pics/BLACKMAGIC%208K.png" width="1000"/>



