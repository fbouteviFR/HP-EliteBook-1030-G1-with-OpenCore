# HP-EliteBook-1030-G1-with-OpenCore

### Status: Running

Currently running:

| Component     | Version      |
| ------------- | ------------ |
| macOS version | 11.3 (20E232) |
| OpenCore      | 0.6.8        |
| BIOS version  | 1.38N86 Ver. 01.44  10/31/2019        |

## Hardware info

| Component | Model                                   |
| --------- | --------------------------------------- |
| CPU       | Intel(R) Core(TM) m5-6Y54 CPU @ 1.10GHz    |
| Memory    | 8GB                       |
| Storage   | KXG50ZNV1T02 TOSHIBA                 |
| Display   | 13.3" 1920x1080                 |
| GPU       | Intel HD Graphics 515                          |
| WLAN      | BCM4352 (replacement of original WIFI Card / eBay) |

## Status

### Working

- [x] Keyboard (including all media keys)
- [x] Battery indicator (number of cycles reported)
- [x] Display brightness (keys F9 and F10)
- [x] Audio
- [x] Ethernet
- [x] iCloud services - iMessage, FaceTime, AppStore
- [x] Camera
- [x] Microphone
- [x] Bluetooth
- [x] Sleep/wake (˜1% of power consumption after 12 hours of sleep)
- [x] Trackpad as a mouse
- [x] HDMI video

## Compatible BIOS settings

| Parameter     | Value      |
| ------------- | ------------ |
| TPM Device | Hidden |
| TPM State | Disable |
| TPM Activation Policy | No prompts |
| Fast Boot | Disable |
| Network (PXE) Boot | Disable |
| Configure Legacy Support and Secure Boot | Legacy Support Disable and Secure Boot Disable |
| HP Application Driver | Disable |
| Wake On LAN | Disabled |
| Extended Idle Power States | Enable |
| Wake when Lid is Opened | Enable |
| Fingerprint Device | Disable |
| Video Memory Size | 128 MB |
| Intel Software Guard Extensions (SGX) | Disable |
| Virtualization Technology (VTx) | Disable |
| Virtualization Technology for Directed I/O (VTd) | Disable |
| Deep Sleep | On |
| Media Card Reader | Disable | 
| Trusted Execution Technology (TXT) | Disable | 
  
## Post-install

sudo pmset autopoweroff 0
sudo pmset powernap 0
sudo pmset standby 0
sudo pmset proximitywake 0
sudo pmset tcpkeepalive 0

## CREDITS

- [Acidanthera](https://github.com/acidanthera)
- [Dortania OC guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [Rehabman's battery patch guide](https://www.tonymacx86.com/threads/guide-how-to-patch-dsdt-for-working-battery-status.116102/) and [Rehabman's ACPI hotpatching guide](https://www.tonymacx86.com/threads/guide-using-clover-to-hotpatch-acpi.200137/)
- [OpenWireless and itlwm](https://github.com/OpenIntelWireless/itlwm)
- Thanks also to Hackintool / great tool
- Thanks also to OpenCore Configurator / great tool too :)
