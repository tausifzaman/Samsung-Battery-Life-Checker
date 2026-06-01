# Samsung Battery Life Checker

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/tausifzaman/Samsung-Battery-Life-Checker/refs/heads/main/assets/logo.png" width="400px;">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/tausifzaman/Samsung-Battery-Life-Checker/refs/heads/main/assets/logo.png" width="400px;">
    <img alt="Samsung Battery Life Checker Logo" src="https://raw.githubusercontent.com/tausifzaman/Samsung-Battery-Life-Checker/refs/heads/main/assets/logo.png" width="400px;">
  </picture>
</div>

<div align="center">

[![Platform](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://github.com/tausifzaman/Samsung-Battery-Life-Checker)
[![Language](https://img.shields.io/badge/Language-Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![Offline](https://img.shields.io/badge/Internet-Not%20Required-success?style=for-the-badge&logo=wifi&logoColor=white)](https://github.com/tausifzaman/Samsung-Battery-Life-Checker)
[![Ads](https://img.shields.io/badge/Ads-None-brightgreen?style=for-the-badge&logo=adblock&logoColor=white)](https://github.com/tausifzaman/Samsung-Battery-Life-Checker)
[![Trackers](https://img.shields.io/badge/Trackers-Zero-brightgreen?style=for-the-badge&logo=shield&logoColor=white)](https://github.com/tausifzaman/Samsung-Battery-Life-Checker)
[![VirusTotal](https://img.shields.io/badge/VirusTotal-Clean%200%2F65-00C853?style=for-the-badge&logo=virustotal&logoColor=white)](https://www.virustotal.com/gui/file/e590422d142466ed0301ab5dfa1a97d939c95903f362d794c4349ab0588c0981)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)
[![Author](https://img.shields.io/badge/Author-Tausif%20Zaman-orange?style=for-the-badge&logo=github)](https://tausifzaman.online)

</div>

---

## Overview

**Samsung Battery Life Checker** is a fully offline Android utility that reads your Samsung device's real battery health, design capacity, and current capacity directly from the system. No internet connection, no account, no ads, and zero data collection.

Most battery apps rely only on standard Android APIs, which often provide limited or inconsistent health information on Samsung devices. This application reads Samsung's actual battery log files to extract accurate data locally on your device.

> Works entirely on-device. Fully offline. No root required. No analytics or third-party SDKs.

---

## Application Information

| Field | Details |
|-------|---------|
| **App Name** | Samsung Battery Life Checker |
| **Package** | `com.tausif.sambchecker` |
| **Platform** | Android |
| **Language** | Kotlin |
| **Minimum SDK** | Android 7.0 (API 24) |
| **Ads / Trackers** | None |
| **Network Required** | No |
| **Device Support** | Samsung Galaxy Devices |
| **VirusTotal** | [0/65 — Clean](https://www.virustotal.com/gui/file/e590422d142466ed0301ab5dfa1a97d939c95903f362d794c4349ab0588c0981) |

---

## Features

- **Real Battery Health Percentage** — reads `mSavedBatteryAsoc` directly from Samsung's dumpstate log, not the simplified Android BatteryManager API
- **Hardware Health Status** — shows actual hardware condition (Good, Overheat, Dead, etc.) from the raw battery health code
- **Samsung Battery Protection** — detects if protection mode is ON and shows the maximum charge threshold (e.g. 85%)
- **Manufacture Date** — reads the real battery manufacture date from `LLB MAN` in the log
- **Voltage & Temperature** — shows exact voltage in mV and temperature in °C/°F with safe range indicators
- **Battery Authenticity Check** — detects if the battery is genuine Samsung or a third-party replacement via `IcAuthenticationResults`
- **Fully Offline** — parses everything locally on your device, no internet required at any step
- **No Account Required** — open the app and check, nothing else
- **No Advertisements** — no ads, now or ever
- **No Trackers** — no Firebase, no Analytics, no Crashlytics
- **Minimal Permissions** — only requests storage access to read the log file, nothing more
- **Lightweight** — under 6MB APK size

---

## Download

Select the correct APK for your device architecture:

| APK | Architecture | Use Case |
|-----|-------------|----------|
| `app-arm64-v8a-release.apk` | ARM 64-bit | Most modern Samsung phones (recommended) |
| `app-armeabi-v7a-release.apk` | ARM 32-bit | Older Samsung devices |
| `app-x86_64-release.apk` | x86 64-bit | Emulators / x86 tablets |
| `app-x86-release.apk` | x86 32-bit | Older emulators |
| `app-universal-release.apk` | Universal | All architectures (larger file) |

<div align="center">

[![Download Latest Release](https://img.shields.io/badge/⬇_Download_Latest_Release-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/tausifzaman/Samsung-Battery-Life-Checker/releases/latest)
&nbsp;
[![GitHub release](https://img.shields.io/github/v/release/tausifzaman/Samsung-Battery-Life-Checker?style=for-the-badge)](https://github.com/tausifzaman/Samsung-Battery-Life-Checker/releases/latest)

</div>

## Screenshots

| Home Screen | Battery Health | Capacity Info |
|:-----------:|:--------------:|:-------------:|
| ![](https://raw.githubusercontent.com/tausifzaman/Samsung-Battery-Life-Checker/refs/heads/main/assets/home.jpg) | ![](https://raw.githubusercontent.com/tausifzaman/Samsung-Battery-Life-Checker/refs/heads/main/assets/battery.jpg) | ![](https://raw.githubusercontent.com/tausifzaman/Samsung-Battery-Life-Checker/refs/heads/main/assets/capacity.jpg) |

---


## Safety and Trust

This application has been independently scanned and verified:

| Check | Result |
|-------|--------|
| VirusTotal Scan | [**0 / 65 — Fully Clean**](https://www.virustotal.com/gui/file/e590422d142466ed0301ab5dfa1a97d939c95903f362d794c4349ab0588c0981) |
| Internet Access | App requests zero internet permission |
| Data Collection | No user data is collected, stored, or transmitted |
| Trackers | No third-party SDKs, analytics, or crash reporters |
| Monetization | No ads, no in-app purchases, no subscriptions |
| Permissions | Only reads battery system stats — nothing else |

You can verify the APK yourself on [VirusTotal](https://www.virustotal.com/gui/file/e590422d142466ed0301ab5dfa1a97d939c95903f362d794c4349ab0588c0981) or decompile it with [jadx](https://github.com/skylot/jadx).

---


## How It Works

Android's standard `BatteryManager` API gives only a simplified "Good / Bad" health answer. Samsung devices write a detailed diagnostic log through `*#9900#` → SysDump → "Run dumpstate/logcat" that contains real battery data most apps never read.

This app parses that log file locally to extract:

```
dumpState_[MODEL]_[DATE].log
  ├── mSavedBatteryAsoc        → real battery health %
  ├── health                   → hardware health code
  ├── voltage                  → battery voltage in mV
  ├── temperature              → battery temperature (×0.1°C)
  ├── mProtectBatteryMode      → Samsung protection mode on/off
  ├── mMaximumProtectionThreshold → max charge limit when protection is on
  ├── LLB MAN                  → battery manufacture date
  └── IcAuthenticationResults  → genuine battery check
```

The file is read directly from `/storage/emulated/0/log/` on your device. Nothing leaves your phone.


---


## Privacy

Samsung Battery Life Checker operates completely offline.

- No internet access required
- No analytics services
- No crash reporting services
- No user accounts
- No cloud synchronization
- No personal data collection

---

## Installation

### Standard Installation

1. Download the correct APK from [Releases](https://github.com/tausifzaman/Samsung-Battery-Life-Checker/releases/latest)
2. On your Samsung device, go to **Settings → Apps → Install Unknown Apps**
3. Allow your browser or file manager to install APKs
4. Open the downloaded APK and tap **Install**
5. Open the app — no setup required

### ADB Installation (Advanced)

```bash
adb install app-arm64-v8a-release.apk
```

---


## FAQ

<details>
<summary>Does the app require root?</summary>

No. The app works without root access.

</details>

<details>
<summary>Does it require an internet connection?</summary>

No. The application works completely offline.

</details>

<details>
<summary>Does it collect user data?</summary>

No. The app does not collect, store, or transmit any user data.

</details>

<details>
<summary>Does it support all Samsung phones?</summary>

Most Samsung Galaxy devices are supported. Compatibility may vary depending on device model and firmware version.

</details>

<details>
<summary>Does it upload battery logs?</summary>

No. All processing happens locally on your device. Nothing is uploaded anywhere.

</details>

<details>
<summary>Can it detect Battery Protection mode?</summary>

Yes. On supported Samsung devices, the app can detect Battery Protection status and charging thresholds.

</details>
<details>
<summary>Does this app work on non-Samsung devices?</summary>

No. The app is specifically designed for Samsung Galaxy devices.

</details>

<details>
<summary>Why does the app need access to log files?</summary>

The application reads Samsung-generated diagnostic logs to extract battery information locally on your device.

</details>


---

## Why This Instead of Play Store Battery Apps?

Most Play Store battery apps:

- Show fake health data (always says "Good") because they only read the basic API
- Require internet to "calculate" what is already stored on your device
- Pack in ad SDKs, Firebase, and tracking libraries
- Ask for unnecessary permissions like contacts, camera, or location
- Gate real diagnostic data behind subscriptions or ads

This app does the opposite of all of that — reads the actual Samsung system log, parses it offline, shows you the real numbers, and does nothing else.


---

## Bug Reports

Found a bug or your device is not showing correct data?

[Open an Issue](https://github.com/tausifzaman/Samsung-Battery-Life-Checker/issues)

Please include:
- Samsung model (e.g., Galaxy S23 Ultra)
- Android version
- What you expected versus what you saw

---

## License

```
MIT License

Copyright (c) 2026 Tausif Zaman

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software.
```

Full license: [LICENSE](LICENSE)

---

## Author

<div align="center">

<img src="https://github.com/tausifzaman.png" width="90" alt="Tausif Zaman"/>

## Tausif Zaman

*Developer · Security Researcher · Tool Builder*

[![Website](https://img.shields.io/badge/🌐_Website-tausifzaman.online-00C853?style=for-the-badge&logoColor=white)](https://tausifzaman.online)
&nbsp;
[![GitHub](https://img.shields.io/badge/GitHub-@tausifzaman-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/tausifzaman)



![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)
![Web%20Security](https://img.shields.io/badge/Web_Security-FF4444?style=flat-square&logo=hackerone&logoColor=white)

</div>

---

## Support

<div align="center">

### If this app helped you understand your battery better —

> ⭐ **Star this repo. It helps others find this tool.**


[![Star on GitHub](https://img.shields.io/github/stars/tausifzaman/Samsung-Battery-Life-Checker?style=for-the-badge&logo=github&label=Star%20this%20repo&color=FFD700&logoColor=white)](https://github.com/tausifzaman/Samsung-Battery-Life-Checker/stargazers)
&nbsp;
[![Follow @tausifzaman](https://img.shields.io/github/followers/tausifzaman?label=Follow%20%40tausifzaman&style=for-the-badge&logo=github&color=00C853&logoColor=white)](https://github.com/tausifzaman)

</div>

---

<div align="center">
<sub>
⚡ Built by <strong>Tausif Zaman</strong> &nbsp;·&nbsp; No ads. No tracking. Just truth about your battery.
</sub>
</div>
