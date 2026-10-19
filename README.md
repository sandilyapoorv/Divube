# Divube

<p align="center">
  <img src="applogo.png" alt="Divube Logo" width="128" style="border-radius: 28px;" />
</p>

<p align="center">
  <strong>Fast, ad-free YouTube streaming client for Android with SponsorBlock, fluid gesture controls, background audio playback, and multi-account sync.</strong>
</p>

<p align="center">
  <a href="https://github.com/sandilyapoorv/Divube/releases"><img src="https://img.shields.io/badge/Release-v1.0.3-blue?style=flat-square" alt="Version"></a>
  <a href="https://github.com/sandilyapoorv/Divube/releases"><img src="https://img.shields.io/badge/Architecture-arm64--v8a-success?style=flat-square" alt="Architecture"></a>
  <img src="https://img.shields.io/badge/Android-7.0%2B%20(API%2024%2B)-orange?style=flat-square" alt="Minimum Android">
  <img src="https://img.shields.io/badge/APK%20Size-~69MB-brightgreen?style=flat-square" alt="Size">
</p>

---

## 📥 Download & Installation

The latest standalone release APK is available under GitHub Releases:

- **Direct Download**: **[`divube-public-release.apk`](https://github.com/sandilyapoorv/Divube/releases/download/v1.0.3/divube-public-release.apk)** (or browse **[All Releases](https://github.com/sandilyapoorv/Divube/releases)**)
- **Minimum Requirement**: Android 7.0 (Nougat / API 24) or newer
- **Architecture**: Modern 64-bit ARM (`arm64-v8a`)

### How to Install:
1. Download **`divube-public-release.apk`** to your Android device.
2. Open the downloaded file from your browser or file manager.
3. If prompted, toggle **"Allow from this source"** to permit installation.
4. Tap **Install** and launch Divube.

---

## ✨ Features

### 🛡️ Pure Ad-Free Experience
- **Zero Ads**: Native network-level filtration strips pre-roll, mid-roll, and banner ads before they ever reach the player.
- **Clean Feeds**: Automatically removes sponsored posts, brand banners, and feed promotions from Home, Search, and Subscriptions.

### ⏭️ SponsorBlock Integration
- Automatically skip sponsored promotional segments, intro sequences, end-cards, and filler content.
- **Customizable Skip Controls**: Configure categories to automatically skip or display a notice.
- **Unskip Option**: 1-tap toast prompt lets you unskip segments whenever you want to watch them.

### 🚀 Direct InnerTube High-Speed Streaming
- **Direct YouTube Engine**: Connects directly to YouTube's official streaming endpoints (`youtubei/v1`) with zero reliance on slow, rate-limited third-party proxy relays.
- **Multi-Tier Stream Resolution**: Employs resilient authenticated playback pipelines with adaptive resolution matching up to 4K 60fps.
- **Session Continuity**: Maintains an active, authorized Google session so playback never drops into unauthenticated bot-challenge walls.

### 🖐️ Fluid Gesture Controls
- **Vertical Swipe for Brightness**: Slide up/down on the left side of the player to adjust screen brightness.
- **Vertical Swipe for Volume**: Slide up/down on the right side of the player to adjust media volume.
- **Double-Tap Seek**: Double-tap on the left or right edge for animated circular ripple seek (`+10s` / `-10s`).
- **Press-to-Speed**: Press and hold anywhere on the screen for instant `2.0x` playback speed.

### 🎧 Background & Picture-in-Picture (PiP)
- **Background Audio**: Keep listening to music or podcasts while your screen is locked or while using other apps.
- **Corner-Docked Miniplayer**: Fluid 16:9 floating miniplayer that smoothly docks to your screen corner while you browse feeds.
- **Picture-in-Picture**: Standard Android PiP mode on supported devices.

### 👥 Seamless Multi-Account Switching
- Google Sign-In with official YouTube session verification.
- Add and manage multiple Google accounts on the same device.
- Instant 1-tap account switching with synchronized cloud watch history, playlists, and subscriptions.

### 📥 High-Speed On-Device Downloader
- Download full videos or audio-only tracks (M4A) directly to local storage.
- Multi-resolution selector (from 144p up to 4K 60fps) with multi-language audio track options.
- Foreground download service with live speed, percentage notifications, and pause/resume/cancel controls.

### 🎨 Deep UI Polish & AMOLED Black
- Full Material 3 dynamic theming supporting System Light, System Dark, and True Pure Black AMOLED modes.
- **Custom Accent Color Wheel**: Pick any custom accent color and saturation level.
- Built entirely with modern Jetpack Compose for buttery-smooth 120Hz scrolling.

---

## 🔒 Privacy & Data Protection

- **Local Storage**: All session data, account tokens, and preferences are stored exclusively on your device in private app storage.
- **No Third-Party Relays**: All streaming and API requests go directly between your device and YouTube servers over encrypted HTTPS.
- **Zero Telemetry Tracking**: No third-party analytics trackers, crashlytics scrapers, or telemetry data collection.

---

## 📄 License & Credits

Distributed for personal and educational use.  
- [SponsorBlock](https://sponsor.ajay.app/) community database for segment timestamps.
- [ExoPlayer (AndroidX Media3)](https://github.com/androidx/media) for playback foundation.
- [yt-dlp](https://github.com/yt-dlp/yt-dlp) for media extraction capabilities.
