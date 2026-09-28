# iBYD Changelog

All notable changes, new features, and improvements to **iBYD** are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.03-beta] - 2026-09-29

### 🎙️ Siri / Apple Intelligence Liquid Aurora Voice Overlay & Audio Focus Ducking
- **Futuristic AI Glass Design**: Redesigned `ListeningOverlay` with glowing liquid AI orb visualizer (cyan, indigo, emerald, neon pink), rotating aura halo, dynamic gradient borders, and frosted glassmorphism styling.
- **Automotive Audio Focus Ducking**: Automatically ducks background vehicle media playback (Spotify, Radio, YouTube) by ~70% during voice listening for crystal-clear microphone audio recording, and restores media volume upon session finish.
- **Dynamic Audio Amplitude Visualizer**: Connected real-time microphone volume (`audioLevel`) directly to GPU hardware-accelerated (`graphicsLayer`) waveform bars.
- **Speaker Voice Calibration Wizard**: Added 5-Sentence Voice Calibration Wizard for driver accent and cadence adaptation with strict sentence verification.
- **Smart Auto-Dismiss & Interactivity**: Added 8-second auto-dismiss timeout after agent responses; touching or dragging the overlay instantly resets/cancels the timer.
- **Screen Boundary Clamping**: Clamped overlay drag coordinates (`x, y`) within screen edges, preventing overlay clipping on automotive head unit displays.
- **Custom Agent Name Support**: Dynamically resolves custom wake/display names set in Settings (`agent_name` in `voice` SharedPreferences, e.g., *"BYD AI"*, *"Jarvis"*).
- **60 FPS Performance Optimization**: Removed `animateContentSize` system window conflicts and replaced smooth scroll coroutines with direct scroll for 100% butter-smooth 60 FPS performance.

---

## [0.02-beta] - 2026-09-28

### 🌟 What's New & Fixed in v0.02-beta

#### 🎨 Navigation Bar & Vehicle Theme Sync
- **System Navigation Bar Integration**: Fixed Vehicle section switching so Android system navigation and status bars dynamically adapt to active iBYD themes (Dark, Daylight `#F3F4F4`, Ocean, Mint, Amber, etc.) without exposing default black bars.

#### 📱 Social Media & TikTok Card Layout Improvements
- **RTL & Theme Adjustments**: Corrected TikTok and Social Media cards alignment, card borders, and font colors to properly render in both LTR and RTL (Arabic/Kurdish) layout modes with full theme compatibility.

#### 🛡️ Stability & Crash Guard Audit
- **Null-Safety Enhancements**: Resolved potential NullPointerException (NPE) crash risks in `ActionDispatcher` context lookups and `PlaceEditDialog` callbacks.
- **Robust Exception Handling**: Enhanced runtime stability across screen rotations, floating overlay view detachments, and ADB command execution background tasks.

---

## [0.01-beta] - 2026-09-28

### 🚀 Welcome to iBYD Beta (v0.01-beta)
**iBYD** is a modern, luxury automotive cockpit, telemetry, and smart assistant application designed specifically for **BYD Electric & Hybrid Vehicles** running on DiLink 3.0, 4.0, and 5.0 systems.

---

### ✨ Key Features & Highlights

#### 📱 1. Split-Screen & Multi-Tasking (Dual-Split)
- **Run Any App Beside Telemetry**: Launch Google Maps, Waze, YouTube, Spotify, or any installed Android app directly inside the iBYD dashboard next to your live car status.
- **Full Touch Support**: Responsive touch input scaling optimized for BYD screens.
- **BYD Rotating Screen**: Seamless transition between landscape (1920x1080) and portrait (1080x1920) modes.

#### 📶 2. Automatic ADB Port Restoration & Wi-Fi Alerts
- **Reboot Auto-Recovery**: Automatically restores classic ADB port 5555 on newer BYD firmwares (`2606+`) where reboot hooks are disabled.
- **Smart Wi-Fi Notifications**: Detects when your car connects to Wi-Fi/Hotspot and sends a status alert when ADB is restored.

#### 🎙️ 3. Hands-Free Offline Voice Agent
- **Button-Free Voice Commands**: Control your car (windows, climate, doors, media) using voice without pressing buttons.
- **Custom Agent Wake Name**: Set a personalized wake name (e.g. *"Leo"* or *"ليون"*).
- **Offline & Private**: Powered by Sherpa-ONNX with full offline support in English & Arabic.

#### 🚗 4. Real-Time Vehicle Telemetry & Model Auto-Detection
- **Live Vehicle Gauges**: Battery State of Charge (SOC), 12V battery voltage, motor power flow, tire pressures (TPMS), and cabin climate.
- **Auto-Model Detection**: Auto-detects your BYD vehicle model (Atto 3, Seal, Han, Tang, Song Plus, Dolphin, Seagull, Denza D9, Qin L, etc.) and adjusts car silhouettes and door indicators.

#### 🎨 5. Luxury Automotive Themes
- **Adaptive Color Palettes**: Choose from Cockpit Dark, Daylight Light (#F3F4F4), Ocean, Amber, Carbon, Redline, Mint, Sky, Coral, or create your own Custom Theme.
- **Full Theme Sync**: Dashboard cards, dialogs, floating widgets, and social sections dynamically adapt to your selected theme.

#### ⚡ 6. Smart Car Automation Rules
- Custom automation triggers for acoustic lock/unlock chimes, automatic window & trunk alerts, and safety notifications.

#### 🌍 7. Multi-Language Support
- Full localization in **8 Languages**: English, Arabic, Sorani Kurdish, Badini Kurdish, Persian, Turkish, Russian, and French.