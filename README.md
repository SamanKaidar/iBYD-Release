# ⚡ iBYD — Smart BYD Assistant & Vehicle Dashboard

[![Release](https://img.shields.io/github/v/release/SamanKaidar/iBYD-Release?style=for-the-badge&color=00E676&label=Latest%20Release)](https://github.com/SamanKaidar/iBYD-Release/releases/latest)
[![Download APK](https://img.shields.io/badge/Download-APK%20(v0.30)-00E676?style=for-the-badge&logo=android)](https://github.com/SamanKaidar/iBYD-Release/releases/download/v0.30/iBYD-v0.30.apk)

Welcome to the official public distribution repository for **iBYD**.

---

## 📥 Direct Download

👉 **[Download iBYD v0.30 APK (Direct Download)](https://github.com/SamanKaidar/iBYD-Release/releases/download/v0.30/iBYD-v0.30.apk)** (~45 MB)

All releases and version history are available on the [**Releases Page**](https://github.com/SamanKaidar/iBYD-Release/releases).

---

## ✨ What's New in v0.30

- ☀️ **Light Mode Visibility Overhaul**:
  - Fixed low-contrast neon texts across Screens, Custom Dials, Settings, and Dashboard tabs.
  - Active screen switcher tabs and filter chips now use daylight-optimized cobalt blue and adaptive card surfaces.
  - Replaced hardcoded dark containers with elevated light surfaces for dial skins, bench test speed bar, and launcher buttons.
- 🔌 **Dedicated ADB Status Pill**:
  - Added a prominent ADB status badge right beside **AEB Active** in the dashboard top bar (`ADB CONNECTED` vs `LOCAL SERVICE`), so the driver can immediately verify communication state.
- 🛡️ **Anti-Force-Stop & Crash Hardening**:
  - Added coroutine exception handlers to `TrackingService.serviceScope` and `IBYDApp.appScope` to safely intercept unexpected coroutine errors before they reach the system crash handler.
  - Hardened `TrackingService.start()` and `startForeground()` against `ForegroundServiceStartNotAllowedException` and background startup restrictions.

---

## 🚀 Installation Guide

1. Download **`iBYD-v0.30.apk`** directly to your phone, PC, or USB flash drive.
2. If using a USB drive, plug it into your BYD DiLink USB port and open the built-in File Manager.
3. Tap on the APK file to install (enable "Install from unknown sources" if prompted).
4. Launch **iBYD** and enjoy the enhanced cockpit experience!
