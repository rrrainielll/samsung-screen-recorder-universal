# Samsung Screen Recorder - Universal Edition

[![Version](https://img.shields.io/badge/version-99.9.99-blue.svg)](https://github.com/rrrainielll)
[![Android](https://img.shields.io/badge/Android-7.0%2B-green.svg)](https://developer.android.com)
[![License](https://img.shields.io/badge/license-Modified-orange.svg)](https://github.com/rrrainielll)

A modified version of Samsung Screen Recorder that works on **all Samsung Android devices** without requiring root access or system signatures.

## 🎯 Features

### Core Features
- ✅ **Universal Compatibility** - Works on all Samsung devices (Android 7.0+)
- ✅ **No Root Required** - Install as a regular app
- ✅ **Screen Recording** - High-quality screen capture with audio
- ✅ **Audio Options** - Mute / System Sounds / System + Microphone
- ✅ **Video Quality** - Low / Medium / High settings
- ✅ **Touch Recording** - Show touch interactions on screen

### New Features
- 🆕 **Hide Floating Button** - Optional: Record without on-screen controls
- 🆕 **Foreground Service** - Reliable recording with persistent notification
- 🆕 **Standard MediaProjection API** - Uses official Android screen capture API

## 📱 Requirements

- **Android Version**: 7.0 (Nougat) or higher
- **Device**: Samsung smartphones/tablets
- **Permissions**: Screen recording, Audio recording, Storage access
- **Root**: Not required

## 📥 Installation

### Method 1: ADB Install
```bash
adb install screenrecorder_customized-aligned-debugSigned.apk
```

### Method 2: Manual Install
1. Download `screenrecorder_customized-aligned-debugSigned.apk`
2. Enable "Install from Unknown Sources" in device settings
3. Open the APK file and install

## 🚀 Usage

# 🚨 <span style="color:red">IMPORTANT NOTE (DO NOT DISREGARD — IT WON’T WORK!)</span>

<span style="color:red">Just press and hold the **Screen Recorder** tile in **Quick Settings**.</span>

<span style="color:red">Once it opens, go to **Recent apps**, tap the **Recorder app icon**, and **allow all required permissions**.</span>


### Starting a Recording

1. Open **Screen Recorder** app
2. Grant screen recording permission when prompted
3. Tap the record button or use Quick Settings tile
4. Recording begins after 3-second countdown

### Settings

Access settings via the menu (⋮) in the app:

- **Record touch interactions** - Show/hide touch points
- **Hide floating button** - Remove on-screen controls (NEW!)
- **Record sound** - Choose audio source
- **Video quality** - Select recording quality

### Stopping a Recording

**With Floating Button** (default):
- Tap the floating stop button

**Without Floating Button** (when hidden):
- Pull down notification shade
- Tap "Tap here to stop recording"

### Viewing Recordings

Recordings are saved to:
```
/storage/emulated/0/DCIM/Video screenshots/
```

## ⚙️ Configuration

### Hide Floating Button

To record without the on-screen floating button:

1. Open Screen Recorder → Settings
2. Enable **"Hide floating button"**
3. Start recording
4. Use notification to stop recording

**Benefits**:
- Cleaner recordings without on-screen controls
- Useful for tutorials and demonstrations
- Notification always available for stopping

## 🔧 Technical Details

### Modifications Made

1. **Removed System Signature Requirement**
   - Allows installation without system privileges
   - No root access needed

2. **Implemented MediaProjection API**
   - Uses standard Android screen capture API
   - Works on all Android 7.0+ devices

3. **Foreground Service Implementation**
   - Reliable recording with persistent notification
   - Complies with Android background service restrictions

4. **Fixed Android Compatibility**
   - Proper `startForegroundService()` usage for Android 8+
   - Foreground notification within 5-second requirement

5. **Added Preference System**
   - Hide floating button toggle
   - Persistent settings storage

### Architecture

```
Screen Recorder
├── MediaProjection API - Screen capture
├── MediaCodec - Video encoding
├── MediaMuxer - Audio/Video muxing
├── FloatingButtonView - Optional on-screen controls
└── ForegroundService - Background recording
```

### Version Information

- **Version**: 99.9.99
- **Version Code**: 999999999
- **Package**: `com.sec.app.screenrecorder`
- **Min SDK**: 24 (Android 7.0)
- **Target SDK**: 28 (Android 9.0)

## 🐛 Known Issues

### Limitations

- **DRM Content**: Protected content (Netflix, etc.) cannot be recorded
- **First Use**: Permission dialog required on first recording
- **Notification**: Persistent notification during recording (Android requirement)
- **Internal Audio**: May be limited on some Android versions

### Workarounds

**Issue**: "Can't record screen" error
- **Solution**: Grant all permissions in app settings

**Issue**: Recording stops immediately
- **Solution**: Clear app cache and restart

**Issue**: No audio in recording
- **Solution**: Select "System sounds + Mic" in settings

## 📖 FAQ

### Q: Why do I need to grant screen recording permission?
**A**: Android requires explicit user consent for screen recording via MediaProjection API. This is a security feature.

### Q: Can I use this on non-Samsung devices?
**A**: This app is specifically modified for Samsung devices. It may not work correctly on other manufacturers' devices.

### Q: Is root required?
**A**: No! This modified version works without root access.

### Q: Why is there a persistent notification during recording?
**A**: Android requires foreground services to show a notification. This ensures the recording service isn't killed.

### Q: Can I record internal audio?
**A**: Yes, select "System sounds" or "System sounds + Mic" in settings. Note: Some apps may block internal audio recording.

## 📄 License

This is a modified version of Samsung Screen Recorder. All modifications are provided as-is for educational purposes.

**Original App**: Samsung Screen Recorder v4.0.23  
**Modified By**: [rrrainielll](https://github.com/rrrainielll)

## 🤝 Contributing

This is a personal modification project. If you have suggestions or improvements:

1. Fork the repository
2. Create your feature branch
3. Submit a pull request

## ⚠️ Disclaimer

This is an unofficial modification of Samsung Screen Recorder. Use at your own risk. The original app is property of Samsung Electronics.

- Not affiliated with Samsung Electronics
- For personal/educational use only
- No warranty provided

## 📞 Support

- **Issues**: Report bugs via GitHub Issues
- **Discussions**: Use GitHub Discussions for questions
- **Updates**: Check repository for latest versions

## 🙏 Acknowledgments

- Samsung Electronics for the original Screen Recorder app
- Android Open Source Project for MediaProjection API
- apktool and uber-apk-signer developers

---

**Modified by [rrrainielll](https://github.com/rrrainielll)** | Version 99.9.99
