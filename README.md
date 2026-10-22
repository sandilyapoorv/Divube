# Divube

<p align="center">
  <img src="applogo.png" alt="Divube Logo" width="128" style="border-radius: 28px;" />
</p>

<p align="center">
  <strong>Fast, ad-free YouTube streaming client for Android with SponsorBlock, fluid gesture controls, background audio playback, and multi-account sync.</strong>
</p>

<p align="center">
  <a href="https://github.com/sandilyapoorv/Divube/releases"><img src="https://img.shields.io/badge/Release-v1.1.0-blue?style=flat-square" alt="Version"></a>
  <a href="https://github.com/sandilyapoorv/Divube/releases"><img src="https://img.shields.io/badge/Architecture-arm64--v8a-success?style=flat-square" alt="Architecture"></a>
  <img src="https://img.shields.io/badge/Android-7.0%2B%20(API%2024%2B)-orange?style=flat-square" alt="Minimum Android">
  <img src="https://img.shields.io/badge/APK%20Size-~5.6MB-brightgreen?style=flat-square" alt="Size">
</p>

---

## 🚀 What's New & Recent Updates

### 🎨 Adaptive Material You & Interactive Color Wheel Studio
- **Dynamic Theming (Material You):** On Android 12+, UI colors automatically harmonize with your device's wallpaper palette.
- **Interactive Color Wheel Picker:** Fine-tune accent hues, intensity, and saturation in real time with an HSV color wheel dialog.
- **True Pure Black AMOLED:** High-contrast pure black mode that saves battery and eliminates pixel glow on OLED screens.
- **Tactile Micro-Interactions:** Delightful bounce-click feedback (`bounceClick`), liquid scale pulses, and party poppers for likes and subscriptions.

### 📑 Complete Google Playlist Management Suite
- **Dedicated Playlists Screen:** Directly view, browse, and organize all playlists created on your signed-in Google account with live video counts and privacy indicators.
- **Create & Edit Playlists:** Easily create brand-new playlists with custom titles, descriptions, and privacy visibility (Public, Unlisted, Private).
- **In-App Playlist Operations:** Edit playlist metadata, reorder or remove individual videos, and delete obsolete playlists with a single tap.
- **1-Tap Save to Playlist:** Intuitive bottom sheet dialog to bookmark any video or stream to one or multiple playlists simultaneously.

### 📂 Public Storage & Zero App-Data Bloat
- **Stored in `/Download/Divube`:** Downloaded videos and audio tracks now automatically save into your device's public `Download/Divube` directory (`/storage/emulated/0/Download/Divube`). They appear instantly in your favorite file manager, gallery, and video player apps.
- **Zero "User Data" Bloat:** Downloaded media is excluded from internal app data in Android Settings, keeping the app's internal footprint minimal regardless of how many videos you download.
- **Automatic Legacy Migration:** Any older downloads stored in internal app-specific directories are smoothly migrated into `/Download/Divube` on launch, immediately freeing up internal storage.
- **Resilient Audio/Video Muxing:** Rock-solid stream merging pipeline that runs smoothly without permission errors across all Android versions (including Android 10+ scoped storage).
- **Accurate File Sizes:** Fixed the 0B file issue—all downloaded files report exact file sizes and metadata immediately upon completion.
- **Pause & Resume Downloads:** Full support for pausing and resuming downloads from both notifications and the in-app Downloads screen.

### 🧹 Automatic Startup Cache Cleaner
- **Fresh Launch Sweep:** Automatically clears temporary download segments, aborted chunks, and `.tmp` files every time the app opens so junk never accumulates.
- **In-App Cache Controls:** Added a "Clear cache on app launch" toggle and a 1-tap "Clear app cache" button with live storage readout in Settings.

### ⚡ HD Shorts Engine with Sub-Second Caching
- **Full HD Visuals:** Shorts now stream in crisp 1080p and 720p HD with perfectly synchronized high-bitrate audio tracks.
- **Instant 0ms Playback:** Dual-player pre-caching with lookahead preloading buffers upcoming shorts in the background for zero-buffering swipes.
- **Flicker-Free Transitions:** Eliminates black screen flashes between shorts with seamless surface continuity.

### 💬 Interactive Rich Comments & Gesture Controls
- **Rich Comments Rendering:** Clickable timestamps automatically seek the player to the exact video second. Full support for hyperlinks, bold, italics, and creator heart badges.
- **HUD Gestures & Seek Ripple:** Smooth vertical swipe sliders for volume and brightness, double-tap ripple seek arcs, and press-and-hold for instant 2.0x playback speed.
- **Optimized "You" Tab:** History section defaults directly to Videos for faster access to your recent watch history.

---

## 📥 Download & Installation

The latest standalone release APK is available under GitHub Releases:

- **Direct Download**: **[`divube-public-release.apk`](https://github.com/sandilyapoorv/Divube/releases/download/v1.1.0/divube-public-release.apk)** (or browse **[All Releases](https://github.com/sandilyapoorv/Divube/releases)**)
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

### 🎨 Dynamic Theming & Color Wheel Studio
- Full Material 3 dynamic theming supporting System Light, System Dark, and True Pure Black AMOLED modes.
- **Custom Accent Color Wheel**: Pick any custom accent color, saturation, and intensity level.
- Built entirely with modern Jetpack Compose for buttery-smooth 120Hz scrolling and tactile bounce-click micro-interactions.

### 📑 Comprehensive Google Playlist Management
- View all playlists created on your Google account in a dedicated, high-performance playlist hub.
- Create, rename, change privacy, and delete playlists directly from the app.
- Save videos to multiple playlists simultaneously with custom bottom sheets.

### 🚀 Direct InnerTube High-Speed Streaming
- **Direct YouTube Engine**: Connects directly to YouTube's official streaming endpoints (`youtubei/v1`) with zero reliance on slow, rate-limited third-party proxy relays.
- **Multi-Tier Stream Resolution**: Employs resilient authenticated playback pipelines with adaptive resolution matching up to 4K 60fps.
- **Session Continuity**: Maintains an active, authorized Google session so playback never drops into unauthenticated bot-challenge walls.

### 🖐️ Fluid Gesture Controls & Precision HUD
- **Vertical Swipe for Brightness**: Slide up/down on the left side of the player to adjust screen brightness.
- **Vertical Swipe for Volume**: Slide up/down on the right side of the player to adjust media volume.
- **Double-Tap Seek**: Double-tap on the left or right edge for animated circular ripple seek (`+10s` / `-10s`).
- **Press-to-Speed**: Press and hold anywhere on the screen for instant `2.0x` playback speed.

### 💬 Interactive Rich Comments
- Clickable timestamps in comments that instantly seek the video to that exact mark.
- Formatted markdown rendering (bold, italics, URLs, hashtags, user handles).
- Full thread replies and creator heart highlights.

### 🎧 Background & Picture-in-Picture (PiP)
- **Background Audio**: Keep listening to music or podcasts while your screen is locked or while using other apps.
- **Corner-Docked Miniplayer**: Fluid 16:9 floating miniplayer that smoothly docks to your screen corner while you browse feeds.
- **Picture-in-Picture**: Standard Android PiP mode on supported devices.

### 👥 Seamless Multi-Account Switching
- Google Sign-In with official YouTube session verification.
- Add and manage multiple Google accounts on the same device.
- Instant 1-tap account switching with synchronized cloud watch history, playlists, and subscriptions.

### 📥 High-Speed On-Device Downloader
- Download full videos or audio-only tracks (M4A) directly to `/Download/Divube`.
- Multi-resolution selector (from 144p up to 4K 60fps) with multi-language audio track options.
- Foreground download service with live speed, percentage notifications, and pause/resume/cancel controls.

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
- [NewPipe Extractor](https://github.com/TeamNewPipe/NewPipeExtractor) for stream extraction capabilities.
