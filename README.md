# ASUS-TUF-F15-FX506HC-Hackintosh-Mac-OS
Fully functional OpenCore EFI configuration for the ASUS TUF Gaming F15 (FX506HC-HN089 &amp;&amp; HN365). Meticulously optimized for macOS 15 Sequoia and macOS 26 Tahoe with all major bugs fully resolved.

# 💻 ASUS TUF Gaming F15 FX506HC Hackintosh EFI

A production-ready, highly optimized OpenCore EFI configuration designed for the **ASUS TUF Gaming F15 (FX506HC)** laptop. This configuration features native support and optimizations for **macOS 15 Sequoia** and **macOS 16 Tahoe**, with all major platform bugs fully resolved.

---

## 🛠️ Hardware Specifications & System Details

| Component | Hardware Specification |
| :--- | :--- |
| **Laptop Model** | ASUS TUF Gaming F15 FX506HC |
| **Processor** | Intel® Core™ i5-11400H (Tiger Lake) |
| **Integrated GPU** | Intel® UHD Graphics (Native layout configured via ACPI mapping) |
| **Dedicated GPU** | NVIDIA GeForce RTX™ 3050 Laptop GPU
| **Audio Codec** | Realtek ALC256 (High Definition Audio via layout-id adjustments) |
| **Wi-Fi & Bluetooth** | MediaTek MT7921 / MT7925 Wireless Network Adapter |
| **Bootloader** | OpenCore (Latest Stable Release) |

---

## 🟢 Status: What Works Perfectly

- ✅ **Graphics Acceleration:** Full UI rendering with Metal acceleration on the native Intel UHD Graphics interface.
- ✅ **Audio & Input Engine:** Internal speakers, headphone jack, and internal microphone running crisp layouts via custom patches.
- ✅ **Trackpad & Input UI:** Fully operational native gesture controls, multi-touch tracking, and complete keyboard short-keys.
- ✅ **Wireless Connectivity:** Stable Wi-Fi connectivity and internal Bluetooth pairings utilizing custom optimized kext implementations (including MediaTek tracking).
- ✅ **Power & Thermal Management:** Pristine CPU idling, battery state indicators mapping correctly, and manual EC fan profile tracking.
- ✅ **System Functions:** Local iServices (iMessage, FaceTime, App Store), native Sleep/Wake triggers, and custom USB port mapping structures.

---

## 📂 Repository Structure Notice

Before deploying, ensure you follow standard OpenCore security practices:
1. **SMBIOS Customization:** Generate your own clean serial numbers, UUIDs, and Board Serials using `GenSMBIOS` before logging into your Apple Account. Do not use raw templates to avoid Apple ID blacklisting.
2. **ACPI Adjustments:** Built-in custom tables are mapped precisely according to the native SSDTTime dumps of the FX506HC structure.

---

## 🚀 Installation & Quick Start

1. Download the latest source or release package from this repository.
2. Format your USB installer's EFI partition to FAT32.
3. Paste the `BOOT` and `OC` directories directly into the root `EFI` folder of that partition.
4. Update the `config.plist` structure with your unique generated SMBIOS credentials.
5. Boot into your system BIOS, disable **Secure Boot**, set SATA Mode to **AHCI**, and initialize via the OpenCore loader interface.

---

## 🤝 Credits & Acknowledgements

