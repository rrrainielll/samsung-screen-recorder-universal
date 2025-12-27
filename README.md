# Samsung Screen Recorder – Universal

[Version](https://img.shields.io/badge/version-99.9.99-blue)

[Android](https://img.shields.io/badge/Android-7.0%2B-green)

A **modified Samsung Screen Recorder** that works on **all Samsung devices (Android 7.0+)** — **no root, no system signature required**.

## ✨ Features

- Works on **all Samsung devices**
- **No root required**
- Screen recording with audio
- Audio options: **Mute / System / System + Mic**
- Video quality: **Low / Medium / High**
- Optional **touch indicators**
- **Hide floating button** (clean recordings)
- Uses **official MediaProjection API**
- Stable **foreground service**

## 📱 Requirements

- Android 7.0+
- Samsung phone or tablet
- Screen, audio, and storage permissions

## 📥 Installation

**ADB**

```bash
adb install screenrecorder_customized-aligned-debugSigned.apk

```

**Manual**

1. Download the APK
2. Enable *Install unknown apps*
3. Install the APK

## 🚨 IMPORTANT (Required)

**Press and hold the Screen Recorder tile in Quick Settings.**

When it opens:

1. Open **Recent apps**
2. Tap the **Recorder app icon**
3. **Allow all permissions**

> Skipping this step will cause the app to fail.
> 

## ▶️ How to Use

1. Open **Screen Recorder**
2. Grant permissions
3. Start recording (3-second countdown)
4. Stop via floating button or notification

## 📁 Output Location

```
/storage/emulated/0/DCIM/Video screenshots/

```

## ⚠️ Limitations

- DRM apps (Netflix, etc.) cannot be recorded
- Persistent notification during recording (Android requirement)
- Internal audio may be limited on some apps

## ℹ️ Info

- **Package**: `com.sec.app.screenrecorder`
- **Version**: 99.9.99
- **Min SDK**: 24 (Android 7.0)
- **Target SDK**: 28

## ⚠️ Disclaimer

Unofficial modification of Samsung Screen Recorder.

Not affiliated with Samsung. Use at your own risk.

**Original app**: Samsung Screen Recorder v4.0.23

**Modified by**: [rrrainielll](https://github.com/rrrainielll)
