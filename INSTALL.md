# Installation Guide

## Requirements

- Windows 7 SP1, 8.1, 10, or 11 (32-bit or 64-bit)
- .NET Framework 4.6.2 (bundled in the installer if not present)
- USB 2.0 or 3.0 port
- Internet connection during driver installation (for Windows Update drivers)

## Step-by-Step

```
1. Download and extract the archive
2. IMPORTANT: Disable Windows Defender before proceeding
   Windows Security → Virus & threat protection → Manage settings
   → Real-time protection: OFF
3. Run ChimeraTool_Setup.exe as Administrator
4. Follow the installer — accept terms, choose install directory
5. When prompted for drivers, click "Install" for each driver package
6. After installer finishes, DO NOT launch ChimeraTool yet
7. Navigate to the Patch\ folder in the extracted archive
8. Run loader.exe as Administrator
9. Wait for "Server bypass activated — Credits: UNLIMITED" message
10. Launch ChimeraTool
```

## Connecting a Device

**Samsung (Download Mode):**
Power off → hold Volume Down + Home (or Volume Down + Volume Up on newer models) + plug USB

**Samsung (ADB Mode):**
Enable Developer Options → USB Debugging → plug USB → accept the RSA key on device

**MTK Devices:**
Power off completely → hold Volume Down → plug USB → device enters BROM/META mode automatically

**Qualcomm (EDL Mode):**
Use EDL cable or short the test points — device should appear as `Qualcomm HS-USB QDLoader 9008` in Device Manager

**Huawei:**
Enable HiSuite mode in Developer Options, or use Emergency Download mode for bootloader-locked devices

## Driver Troubleshooting

If your device isn't detected:
1. Open Device Manager → look for unknown devices with yellow exclamation marks
2. Right-click → Update Driver → Browse my computer
3. Point to `C:\Program Files\ChimeraTool\Drivers\`
4. Windows will install the correct driver for your device chipset
