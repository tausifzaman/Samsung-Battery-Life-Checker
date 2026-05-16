# Samsung Battery Life Checker

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/tausifzaman/Samsung-Battery-Life-Checker/refs/heads/main/assets/logo.png" width="500px;">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/tausifzaman/Samsung-Battery-Life-Checker/refs/heads/main/assets/logo.png" width="500px;">
    <img alt="Samsung Battery Life Checker Logo" src="https://raw.githubusercontent.com/tausifzaman/Samsung-Battery-Life-Checker/refs/heads/main/assets/logo.png" width="500px;">
  </picture>
</div>

<div align="center">


<br/>

[![Platform](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://github.com/tausifzaman/Samsung-Battery-Life-Checker)
[![Language](https://img.shields.io/badge/Language-Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![Offline](https://img.shields.io/badge/Internet-Not%20Required-success?style=for-the-badge&logo=wifi&logoColor=white)](https://github.com/tausifzaman/Samsung-Battery-Life-Checker)
[![Ads](https://img.shields.io/badge/Ads-None-brightgreen?style=for-the-badge&logo=adblock&logoColor=white)](https://github.com/tausifzaman/Samsung-Battery-Life-Checker)
[![Trackers](https://img.shields.io/badge/Trackers-Zero-brightgreen?style=for-the-badge&logo=shield&logoColor=white)](https://github.com/tausifzaman/Samsung-Battery-Life-Checker)
[![VirusTotal](https://img.shields.io/badge/VirusTotal-Clean%200%2F65-00C853?style=for-the-badge&logo=virustotal&logoColor=white)](https://www.virustotal.com/gui/file/e590422d142466ed0301ab5dfa1a97d939c95903f362d794c4349ab0588c0981)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)
[![Author](https://img.shields.io/badge/Author-Tausif%20Zaman-orange?style=for-the-badge&logo=github)](https://tausifzaman.online)

<br/>

</div>

---

## 📌 Overview

**Samsung Battery Life Checker** is a **100% offline** Android utility that reads your Samsung device's real battery health, design capacity, and current capacity — directly from the system, with no internet connection, no account, no ads, and zero data collection.

Many battery apps rely only on standard Android APIs, which often provide limited or inconsistent health information on Samsung devices.

> ✅ Works entirely on-device. Fully offline. No root. No analytics or third-party SDKs.

---

## 📱 App Info

| Field | Details |
|-------|---------|
| **App Name** | Samsung Battery Life Checker |
| **Package** | `com.tausif.sambchecker` |
| **Platform** | Android |
| **Language** | Kotlin |
| **Min SDK** | Android 7.0 (API 24) |
| **Ads, Trackers** | ❌ None |
| **Offline** | ✅ Fully Offline |
| **Device Support** | Samsung Galaxy Devices |
| **VirusTotal** | [0/65 — Clean ✅](https://www.virustotal.com/gui/file/e590422d142466ed0301ab5dfa1a97d939c95903f362d794c4349ab0588c0981) |

---

## 🔋 Features

- ✅ **Real Battery Health %** — reads from Samsung system logs, instead of relying solely on the limited standard Android BatteryManager API
- ✅ **Design Capacity** — the original mAh your battery was manufactured with
- ✅ **Current Maximum Capacity** — how much your battery can actually hold now
- ✅ **Battery Wear Level** — how degraded your battery is over time
- ✅ **Charge Cycle Estimation** — approximate charge cycles used
- ✅ **100% Offline** — works with no Wi-Fi, no mobile data, no internet at all
- ✅ **No Account Required** — open the app and check, nothing else
- ✅ **No Ads** — not a single ad, not ever
- ✅ **No Trackers** — no Firebase, no Analytics, no Crashlytics, nothing
- ✅ **No Permissions Abuse** — only reads what it needs, nothing more
- ✅ **Lightweight** — under 6MB APK size

---

## 📥 Download

> Choose the correct APK for your device architecture:

| APK | Architecture | Use Case |
|-----|-------------|----------|
| `app-arm64-v8a-release.apk` | ARM 64-bit | ✅ Most modern Samsung phones (recommended) |
| `app-armeabi-v7a-release.apk` | ARM 32-bit | Older Samsung devices |
| `app-x86_64-release.apk` | x86 64-bit | Emulators / x86 tablets |
| `app-x86-release.apk` | x86 32-bit | Older emulators |
| `app-universal-release.apk` | Universal | All architectures (larger file) |

👉 **[Download Latest Release →](https://github.com/tausifzaman/Samsung-Battery-Life-Checker/releases/latest)**

---

## 🛡️ Safety & Trust

This app has been independently scanned and verified:

| Check | Result |
|-------|--------|
| 🔬 VirusTotal Scan | [**0 / 65 — Fully Clean**](https://www.virustotal.com/gui/file/e590422d142466ed0301ab5dfa1a97d939c95903f362d794c4349ab0588c0981) |
| 🌐 Internet Access | ❌ App requests zero internet permission |
| 📊 Data Collection | ❌ No user data is collected, stored, or transmitted |
| 📡 Trackers | ❌ No third-party SDKs, analytics, or crash reporters |
| 💰 Monetization | ❌ No ads, no in-app purchases, no subscriptions |
| 🔐 Permissions | Only reads battery system stats — nothing else |

> You can verify the APK yourself on [VirusTotal](https://www.virustotal.com/gui/file/e590422d142466ed0301ab5dfa1a97d939c95903f362d794c4349ab0588c0981) or decompile it with [jadx](https://github.com/skylot/jadx).

---

## ⚙️ How It Works

Android exposes a **hidden battery stats log** that Samsung devices write with real health data. Most apps ignore this and only read the basic `BatteryManager` API, which gives a simplified "Good / Bad" answer.

This app reads Samsung's actual battery log files to extract:

```
/sys/class/power_supply/battery/
  ├── capacity           → current charge %
  ├── health             → raw health status
  ├── batt_misc_event    → Samsung diagnostic data
  └── ...
```

The data is parsed locally on your device. Nothing leaves your phone.

---

## 📲 Installation

### Normal Install
1. Download the correct APK from [Releases](https://github.com/tausifzaman/Samsung-Battery-Life-Checker/releases/latest)
2. On your Samsung device, go to **Settings → Apps → Install Unknown Apps**
3. Allow your browser or file manager to install APKs
4. Open the downloaded APK and tap **Install**
5. Open the app — no setup required

### ADB Install (Advanced)
```bash
adb install app-arm64-v8a-release.apk
```

---

## 📸 Screenshots

<!-- Add your screenshots inside the /screenshots folder and update these paths -->

| Home Screen | Battery Health | Capacity Info |
|:-----------:|:--------------:|:-------------:|
| *(screenshot)* | *(screenshot)* | *(screenshot)* |

---

## 🤔 Why Not Use Play Store Battery Apps?

Most Play Store battery apps:

- ❌ Show fake health data (always says "Good")
- ❌ Require internet to "calculate" what's already on your device
- ❌ Pack in many trackers and ad SDKs
- ❌ Ask for permissions they don't need
- ❌ Gate real data behind subscriptions

This app does the opposite of all of that.

---

## 🐛 Bug Reports

Found a bug or your device isn't showing correct data?

👉 [Open an Issue](https://github.com/tausifzaman/Samsung-Battery-Life-Checker/issues)

Please include:
- Samsung model (e.g. Galaxy S23 Ultra)
- Android version
- What you expected vs what you saw

---

## 📄 License

```
MIT License

Copyright (c) 2026 Tausif Zaman

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software.
```

Full license: [LICENSE](LICENSE)

---

## 👤 Author

<div align="center">

**Tausif Zaman**

🌐 [tausifzaman.online](https://tausifzaman.online) &nbsp;·&nbsp; 🐙 [GitHub @tausifzaman](https://github.com/tausifzaman)

*Android Developer · Security Researcher · Tool Builder*

Kotlin · Python · PHP · Android · Web Security

</div>

---

## ⭐ Support

If this app helped you understand your battery better:

<div align="center">

⭐ **Star this repo to help others find it!** ⭐

[![Star](https://img.shields.io/github/stars/tausifzaman/Samsung-Battery-Life-Checker?style=social)](https://github.com/tausifzaman/Samsung-Battery-Life-Checker)
&nbsp;
[![Follow](https://img.shields.io/github/followers/tausifzaman?style=social)](https://github.com/tausifzaman)
&nbsp;
[![Website](https://img.shields.io/badge/Visit-tausifzaman.online-blue?style=flat-square)](https://tausifzaman.online)

</div>

---

<div align="center">
<sub>Made with ❤️ by <a href="https://tausifzaman.online">Tausif Zaman</a> — No ads. No tracking. Just truth about your battery.</sub>
</div>
