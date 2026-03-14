# Gigabyte Z370 AORUS 2.0 + i7-8700K Hackintosh (macOS Sonoma 14.3.1)

A complete **OpenCore EFI configuration** for running **macOS Sonoma 14.3.1** on **Gigabyte Z370 AORUS 2.0** with **Intel Core i7-8700K** and **RX Vega 64**.

This repository includes a ready-to-use **EFI folder**, configured and tested with **OpenCore 1.0.6**.

> ⚠️ **Important**  
> Serial numbers, MLB, and other hardware identifiers have been removed. You must generate your own SMBIOS before using this EFI.

---

# System Specifications

| Component | Model |
|---|---|
| **macOS Version** | macOS Sonoma 14.3.1 |
| **Bootloader** | OpenCore 1.0.6 |
| **Motherboard** | Gigabyte Z370 AORUS 2.0 |
| **CPU** | Intel Core i7-8700K |
| **RAM** | 32GB DDR4 3200MHz |
| **GPU** | ASUS RX Vega 64 STRIX 8GB |
| **Storage** | ADATA 256GB SSD |
| **SMBIOS** | iMacPro19,1 (2019) |

---

# Working Features

All core hardware has been tested and works properly.

| Feature | Status |
|---|---|
| macOS Sonoma 14.3.1 | ✅ Working |
| CPU Power Management | ✅ Working |
| GPU Acceleration | ✅ Native Fully Working |
| USB Ports | ✅ Working |
| Thunderbolt | ✅ Working |
| Audio | ✅ Working |

---

# BIOS Settings

Recommended BIOS settings before installing macOS.

### Disable

- VT-d *(unless using proper patches)*
- Fast Boot
- Secure Boot
- CSM

### Enable

- XHCI Hand-off
- Above 4G Decoding
- EHCI/XHCI Hand-off
- SATA Mode → **AHCI**

---

# Required Tools

### OCAuxiliaryTools
https://github.com/ic005k/OCAuxiliaryTools  

Used to edit and manage **OpenCore config.plist**.

### Intel Power Gadget
https://github.com/trulyspinach/SMCAMDProcessor  

Used for monitoring **CPU power usage and performance**.

### Hackintool
https://github.com/headkaze/Hackintool  

Useful for verifying system configuration, USB mapping, and hardware status.

---

# OpenCore Guide

Official documentation for OpenCore installation:

https://dortania.github.io/OpenCore-Install-Guide/

---

# Kext List

Main kexts used in this EFI:

- Lilu.kext
- VirtualSMC.kext
- WhateverGreen.kext
- AppleALC.kext
- IntelMausi.kext
- USBMap.kext

Additional kexts may be included depending on configuration updates.

---

# EFI Folder Structure

```
EFI
├── BOOT
│   └── BOOTx64.efi
│
└── OC
    ├── ACPI
    ├── Drivers
    ├── Kexts
    ├── Resources
    ├── Tools
    └── config.plist
```

---

# Notes

- This EFI is **specifically configured for the hardware listed above**.
- If your hardware differs, you may need to modify:
  - **ACPI**
  - **USB mapping**
  - **config.plist**
- Always generate your own **SMBIOS values** using **GenSMBIOS**.

---

# Disclaimer

This repository is intended for **educational purposes only**.  
Use it at your own risk. The author is not responsible for any hardware or software issues.
