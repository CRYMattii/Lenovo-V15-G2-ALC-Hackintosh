# Lenovo-V15-G2-ALC-Hackintosh
OpenCore EFI for Lenovo V15 G2 ALC — For the latest versions of macOS
# Lenovo V15 G2 ALC Hackintosh

OpenCore EFI for **Lenovo V15 G2 ALC (82KD)**.

This EFI has been tested with **macOS Sequoia 15** and **macOS Tahoe 26**.

## Hardware

| Component | Model |
| --- | --- |
| CPU | AMD Ryzen 3 5300U |
| GPU | AMD Radeon Graphics |
| RAM | 12 GB DDR4 |
| Storage | NVMe SSD |
| Keyboard | PS/2 |
| Trackpad | I2C |
| Wi-Fi | Realtek RTL8822CE |
| SMBIOS | iMac20,1 |

## macOS Compatibility
| --- | --- |
| **macOS Tahoe 26** | ✅ Tested |
| **macOS Sequoia 15** | ✅ Tested |
| macOS Sonoma 14 | ⚠️ Compatible, not tested |
| macOS Ventura 13 | ⚠️ Compatible, not tested |

The EFI has been personally tested with **macOS Sequoia and macOS Tahoe**.

Sonoma and Ventura should also be compatible, but they have not been tested with the current EFI, so correct operation is **not guaranteed**.

## OpenCore GUI

A **clean and elegant graphical interface** has been added to the OpenCore boot picker, replacing the standard text-based menu.

It gives the boot process a much more polished and macOS-like appearance.

<!-- Add your OpenCore GUI screenshot here -->
<!-- ![OpenCore GUI](Images/OpenCore-GUI.jpg) -->

## Wi-Fi

The required **RealtekRTL8822C kext,is already included and configured in the EFI**.

To use Wi-Fi, you only need to download and install **RealtekRTL8822CMenu.app**:

**[RealtekRTL8822C v0.0.5 by flany-dev](https://github.com/flany-dev/RealtekRTL8822C/releases/tag/v0.0.5)**

There is no need to install the kext separately.

After installing the application, open it and use the menu bar icon to connect to your Wi-Fi network.

## Bluetooth on macOS Tahoe

Bluetooth works correctly on **macOS Sequoia 15**.

It currently **does not work exclusively on macOS Tahoe 26**.

A solution for Bluetooth support on Tahoe is currently being investigated. If a working fix is found, the EFI will be updated.

## Hardware Check

Tested using **MacHWCheck Lite**:

```text
============================================================
 MacHWCheck Lite — macOS / Hackintosh quick diagnostics
============================================================

✅ CPU                 AMD Ryzen 3 5300U with Radeon Graphics
✅ RAM                 12 GB
ℹ️ SMBIOS              iMac20,1

✅ Audio               Detected
✅ Webcam              Detected
➖ Wi-Fi               Requires RealtekRTL8822CMenu
✅ Ethernet            Detected
✅ Bluetooth           Detected*
✅ GPU / Display       Detected
✅ Keyboard            Detected
✅ Trackpad            Detected
✅ Battery             Detected
⚠️ USB                 Not verified
✅ NVRAM               Accessible

SIP: Custom Configuration
