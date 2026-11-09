# AppVault 📦

Welcome to **AppVault** — the official distribution repository for production Android APK releases developed by [@abishek-dg](https://github.com/abishek-dg).

---

## 🚀 Available Applications

### 🎮 FEB (Fast ESP32 Bluetooth) Controller
**FEB** is a production-grade, offline Android application engineered for simultaneous multi-device robotics and microcontroller automation over **Bluetooth Low Energy (Nordic UART Service)** and **Classic Bluetooth (SPP RFCOMM)**.

- **APK File**: [`FEB.apk`](./FEB.apk)
- **Version**: `1.0.3` (Build `4`)
- **Package Name**: `com.feb.app`
- **Minimum OS**: Android 7.0 (API 24)
- **Target OS**: Android 14 (API 34)
- **File Size**: `55.20 MB` (`57,885,364` bytes)
- **Signing**: Release Signed (v1, v2, and v3 schemes verified)
- **SHA-256 Checksum**:
  ```text
  925790CAFB5A2DEA778C596E2D4EEBE7126B63F617183E6A762734EF4B21C4E4
  ```

---

## 📥 Installation Guide

1. Download **[`FEB.apk`](./FEB.apk)** directly from this repository or from the [Releases](https://github.com/abishek-dg/AppVault/releases) section.
2. On your Android phone, locate the downloaded APK in your **Downloads** or File Manager.
3. Tap **FEB.apk** to begin installation:
   - If prompted with *"Install unknown apps"*, toggle **Allow from this source** for your browser or file manager.
   - If prompted by Google Play Protect, tap **Install anyway** or **Install** (the release is signed and clean of background admin or accessibility services).
4. Launch **FEB** from your home screen.

---

## ⚡ Key Highlights of FEB

- **Multi-Device Swarm Control**: Connect and broadcast commands to multiple ESP32 and microcontroller boards in parallel (`Future.wait`) without manual device switching.
- **Dual Transport Engine**:
  - BLE Nordic UART Service (`6E400001-B5A3-F393-E0A9-E50E24DCCA9E`)
  - Classic Bluetooth SPP RFCOMM (`00001101-0000-1000-8000-00805F9B34FB`)
- **Free Fire Style Custom HUD Editor**: Move, resize, and position buttons, sliders, and controls with custom snapping and live visual guides.
- **Dual Analog Joystick Modes**:
  - **Mode 1 (Axis-Tagged)**: Outputs clean `X:<val>` and `Y:<val>` streams with directional deadzone clamping.
  - **Mode 2 (XY-Packet)**: Outputs atomic `J:<x>,<y>` packets ideal for omni-directional robotics and differential drive chassis.
- **Independent State Machine & Failsafe**: Per-device emergency stop commands and configurable communication watchdog failsafes.
- **Integrated Live Terminal**: Full 2000-line color-coded monospace terminal with UTF-8 and raw HEX byte inspectors.

---

## 🔒 Verification & Integrity

To verify the APK hash on Windows PowerShell:
```powershell
Get-FileHash -Algorithm SHA256 .\FEB.apk
```

On Linux or macOS:
```bash
sha256sum FEB.apk
```

Expected Output:
```text
925790CAFB5A2DEA778C596E2D4EEBE7126B63F617183E6A762734EF4B21C4E4
```
