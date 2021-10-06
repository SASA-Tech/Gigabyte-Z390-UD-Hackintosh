# Gigabyte-Z390-UD-Hackintosh
[![](https://img.shields.io/badge/Gitter%20HL%20Community-Chat-informational?style=flat&logo=gitter&logoColor=white&color=ed1965)](https://gitter.im/Hackintosh-Life-IT/community)
[![](https://img.shields.io/badge/Repository-SASATech-informational?style=flat&logo=apple&logoColor=white&color=9debeb)](https://github.com/SASA-Tech?tab=repositories)
[![](https://img.shields.io/badge/Telegram-HackintoshLifeIT-informational?style=flat&logo=telegram&logoColor=white&color=5fb659)](https://t.me/HackintoshLife_it)
[![](https://img.shields.io/badge/Facebook-HackintoshLifeIT-informational?style=flat&logo=facebook&logoColor=white&color=3a4dc9)](https://www.facebook.com/hackintoshlife/)
[![](https://img.shields.io/badge/Instagram-HackintoshLifeIT-informational?style=flat&logo=instagram&logoColor=white&color=8a178a)](https://www.instagram.com/hackintoshlife.it_official/)
#### *Leggilo in un'altra lingua: [Italiano](README.md).* :it:

# Italian Repository 🇮🇹
#### macOS Big Sur/Monterey successfully installed on Gigabyte Z390 UD

# Specifiche:

| Components       | Models                             |
| ---------------- | ---------------------------------- |
| Motherboard      | Gigabyte Z390 UD (BIOS 10K)        | 
| CPU              | Intel i5 9400                      | 
| iGPU             | Intel® UHD Graphics 630            |
| Audio            | Realtek ALC887                     |
| RAM              | 16 Gb DDR4 3200 Mhz                |
| SSD              | Samsung 750 Evo 250gb              |
| SMBIOS           | iMac19,1                           |
| Bootloader       | OpenCore 0.7.4                     |

![infodp1](./Screenshot/Mobo.png)

## By default the OC GUI is set to 1920x1080.
If you have a different resolution, go to EFI> OC, delete the Resources folder and unzip the one you need.

## If you want to install macOS Monterey Beta 8:
~~I leave you the config.plist renamed to configbeta8.plist ready to use ONLY to download and install the update. At the end of the update you have to delete it and put back the original config.plist. It is advisable to disconnect the Hackintosh from the Apple ID before temporarily replacing the config.plist, alternatively use the kexts RestrictEvents.~~

This update issue has been fixed with OpenCore 0.7.4. Now you can update without RestrictEvents.kexts and without changing config.plist

## NOTE:
Kexts updated to the latest versions except RealtekRTL8111 which in version 2.4.2 gave problems of instability to the LAN connection at least in my case.

# BIOS Settings:

## Disable:

- Fast Boot
- VT-d
- CSM
- Intel SGX
- Intel Platform Trust
- CFG Lock (MSR 0xE2 write protection)

## Enable:

- Intel Virtualizzation Technology
- Above 4G decoding
- Hyper-Threading
- Execute Disable Bit
- EHCI/XHCI Hand-off
- OS type: (Windows 10 Feautres: Windows 8/10 WHQL oppure Other)
- DVMT Pre-Allocated(iGPU Memory): 64 MB
- DVMT Total Gfx Mem → MAX

## Generic settings, you may not find some.
  
# Dispositivo Screenshot
![infodp1](./Screenshot/Peripherials.png)
![infodp2](./Screenshot/PCIe.png)

# Cosa funziona e cosa no:
- [x] Intel UHD 630 iGPU
- [x] ALC887 internal output
- [x] ALC887 HDMI Audio Output
- [x] USB Ports
- [x] Realtek 8118 Gaming LAN
- [x] NVRAM
- [x] Boot Windows by OpenCore

# Info SSDT Gigabyte Z390 UD

![SSDT](./Screenshot/SSDT.png)

## Credits

- [Acidanthera](https://github.com/acidanthera) for OpenCore Bootloader
- [Apple](https://apple.com) for macOS;
- [HackintoshLifeIT](https://github.com/Hackintoshlifeit) Support group for pre and post installation
- [Baio1977](https://github.com/Baio1977) for the support
- [Lorys89](https://github.com/Lorys89) for the support
- [Dortania](https://github.com/dortania) for OpenCore guides

# If you need help contact us on [Telegram](https://t.me/HackintoshLife_it)
