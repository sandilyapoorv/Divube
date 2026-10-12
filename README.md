# Divube

<p align="center">
  <img src="app/src/main/res/drawable/applogo.png" alt="Divube Logo" width="128" style="border-radius: 28px;" />
</p>

<p align="center">
  <strong>Fast, ad-free YouTube streaming client for Android with SponsorBlock, fluid gesture controls, background audio playback, and multi-account sync.</strong>
</p>

<p align="center">
  <a href="https://github.com/sandilyapoorv/Divube/releases"><img src="https://img.shields.io/badge/Release-v1.0.2-blue?style=flat-square" alt="Version"></a>
  <a href="https://github.com/sandilyapoorv/Divube/releases"><img src="https://img.shields.io/badge/Architecture-arm64--v8a-success?style=flat-square" alt="Architecture"></a>
  <img src="https://img.shields.io/badge/Android-7.0%2B%20(API%2024%2B)-orange?style=flat-square" alt="Minimum Android">
  <img src="https://img.shields.io/badge/APK%20Size-~72MB-brightgreen?style=flat-square" alt="Size">
</p>

---

## ✨ Features

### 🛡️ Ad-Free Experience & uBlock Filtering
- **Zero Ads**: Native network-level filtration strips pre-roll, mid-roll, and banner ads before they ever reach the player.
- **Clean Feeds**: Automatically purges promoted video items, `adSlotRenderer`, `inFeedAdLayoutRenderer`, and brand sponsor placements from Home, Search, and Subscriptions.

### ⏭️ SponsorBlock Integration
- Automatically skip sponsor segments, intro animations, outro end-cards, self-promotions, and off-topic fillers.
- **Customizable Skip Settings**: Individually configure which categories to automatically skip or display a notice for.
- **Unskip Pill**: Displays a discreet notice with a 1-tap "Unskip" option if you want to watch the segment.

### 🖐️ ReVanced Extended Fluid Gestures
- **Swipe for Brightness**: Slide vertically on the left side of the player to adjust screen brightness.
- **Swipe for Volume**: Slide vertically on the right side of the player to adjust media volume.
- **Double-Tap Seek**: Double-tap on the left or right edge for animated circular ripple seek (`+10s` / `-10s`).
- **Press-to-Speed**: Press and hold anywhere on the video for instant `2.0x` speed acceleration.

### 🎧 Background & Picture-in-Picture Playback
- **Background Audio**: Keep listening when locking your screen or switching between apps.
- **Corner-Docked Miniplayer**: Smooth, fluid 16:9 floating miniplayer that docks to your preferred corner while you browse feeds.
- **Picture-in-Picture (PiP)**: Standard Android PiP mode on supported devices.

### 👥 Multi-Account Support
- Seamless Google Sign-In with official YouTube web session verification.
- Add and manage multiple accounts simultaneously.
- 1-tap fast switching between accounts with synchronized cloud watch history, subscriptions, and playlists.

### 🎨 Deep UI Polish & AMOLED Themes
- Full Material 3 theming supporting System Light, System Dark, and True Pure Black AMOLED modes.
- **Custom Accent Color Wheel**: Dial in your preferred accent colors and intensity.
- Responsive modern YouTube-grade layout built entirely in Jetpack Compose.

### ⚡ Lightweight Architecture
- Specially tailored for modern 64-bit devices (`arm64-v8a`), cutting unnecessary multi-ABI binary overhead from **224MB down to ~72MB**.

---

## 📥 Download & Installation

1. Navigate to the **[Releases](https://github.com/sandilyapoorv/Divube/releases)** section.
2. Download the latest `app-release-v8.apk`.
3. Open the APK on your Android device (Android 7.0+ / API 24 or newer).
4. Allow installation from unknown sources if prompted, and install.

---

## 🛠️ Tech Stack & Architecture

- **Language**: Kotlin 1.9.24 / JVM 17
- **UI Framework**: Jetpack Compose + Material 3
- **Media Engine**: ExoPlayer 1.3.1 (Media3) with customized `DefaultLoadControl` buffer strategies
- **Network / API**: OkHttp 4.12, Gson, InnerTube API parser
- **Downloader Engine**: Embedded lightweight `yt-dlp` runtime with native Python and FFmpeg binaries
- **Image Loading**: Coil 2.6.0 with memory and disk caching
- **Build System**: Gradle 8.7 with Android Gradle Plugin 8.3.2

---

## ⚙️ Building from Source

To compile the APK locally using the Android SDK:

```bash
# Clone the repository
git clone https://github.com/sandilyapoorv/Divube.git
cd Divube

# Build the arm64-v8a Release APK
./gradlew assembleRelease --no-daemon

# The output APK will be located at:
# app/build/outputs/apk/release/app-release.apk
```

---

## 🔒 Privacy & Permissions

Divube connects directly to YouTube services via standard HTTPS connections. Your login cookies are stored safely on your device in private app storage (`EncryptedSharedPreferences`) and are never routed through any external proxy or third-party servers.

---

## 📄 License & Credits

Distributed for personal and educational use.  
- [SponsorBlock](https://sponsor.ajay.app/) community database for segment timestamps.
- [ExoPlayer (AndroidX Media3)](https://github.com/androidx/media) for playback foundation.
- [yt-dlp](https://github.com/yt-dlp/yt-dlp) for media extraction capabilities.
