# ECHOES - Pro Audio Streaming Suite 🎧⚡

A sleek, high-fidelity progressive music streaming application crafted with a custom Deep Space & Platinum Silver aesthetic. ECHOES delivers an intuitive, mobile-optimized experience with real-time discovery, intelligent listening history recommendations, system audio routing, and seamless playlist curation.

---

## 🌟 Key Features

### 1. 🎯 Intelligent Personalization & Play History
- **"Listen Again" Shelf**: Stores your recently played tracks (cover art, track name, and artist) in browser `localStorage`. Pick up exactly where you left off or clear the history anytime with one click.
- **Smart "Made for You" Discovery**: Dynamically recommends tracks inspired by your latest listening habits.
- **Text-Only Mood Chips**: Fast vibe switching across `All Vibes`, `Energy`, `Relax`, `Romance`, `Party`, and `Focus` without emoji clutter.

### 2. 🎛️ Real Audio Output & Volume Control
- **Genuine Device Routing**: Inspects and queries real system hardware outputs (`audiooutput` devices) using the Web MediaDevices API and routes audio via `setSinkId` where supported.
- **Dedicated Volume Controller**: Output volume slider with real-time percentage feedback (`0%` to `100%`) and one-click smart mute/unmute that remembers your previous level.
- **Clean Interface**: Volume and output controls are consolidated within the **Audio Output** modal, leaving the full-screen player uncluttered.

### 3. 🔍 Instant Search Engine
- **Live Debounced Search**: Automatically queries the iTunes catalog as you type (with a 300ms debounce to prevent redundant network requests).
- **Instant Enter Execution**: Press `Enter` on physical or mobile keyboards to search immediately.
- **Clear Trigger**: One-tap `X` button clears the search query and restores the default prompt.

### 4. 📜 Stationary Lyrics View
- **Clean Typography**: Readable stationary lyrics formatted with uniform styling (`Plus Jakarta Sans`).
- **No Forced Auto-Scroll**: Eliminates unexpected jumping or shifting, giving you full manual scrolling control.

### 5. 📂 Full Playlist Management & Deletion
- **Custom Playlists**: Create unlimited playlists directly in your library.
- **Full Deletion**: Delete entire custom playlists with confirmation modals (`Liked Songs` remains protected).
- **Track Removal**: Remove individual songs from any custom playlist with one tap.
- **Play All**: One-click streaming for any playlist or curated pack.

### 6. 🎧 Playback Controls & Carousels
- **Shuffle & Loop**: Randomize tracks or repeat the active song with visual state indicators.
- **Floating Mini Player Pill**: Sleek floating bar with animated progress line above the bottom navigation.
- **6 Content Carousels**:
  1. *Listen Again* (History)
  2. *Made for You* (Personalized)
  3. *Recommended Playlists* (Curated packs)
  4. *Trending Today* (Global charts)
  5. *Chill & Lo-Fi Lounge* (Mellow study beats)
  6. *High Energy Workout* (Gym phonk & bass)
  7. *Bollywood & Desi Melodies* (Romantic acoustics)

---

## 🛠️ Tech Stack

- **Markup & Logic**: HTML5, Vanilla JavaScript (ES6+ async/await)
- **Styling**: Tailwind CSS (CDN), FontAwesome 6.4.0 Icons, Google Fonts (`Plus Jakarta Sans`)
- **APIs**:
  - [iTunes Search API](https://developer.apple.com/library/archive/documentation/AudioVideo/Conceptual/iTuneSearchAPI/index.html) (Audio streams & catalog metadata)
  - [Lyrics.ovh API](https://lyricsovh.docs.apiary.io/) (Song lyrics)
  - [Web MediaDevices API](https://developer.mozilla.org/en-US/docs/Web/API/MediaDevices/enumerateDevices) (Hardware audio output detection)
- **Persistence**: Browser `localStorage` (Playlists, Liked Songs, Listen Again history)

---

## 🚀 Quick Start Guide

### Running Locally
1. Clone or download the repository files:
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
   ```
2. Open `index.html` in any modern web browser (Google Chrome, Microsoft Edge, Safari, Firefox, or Brave).
3. Search for any song or tap a recommended playlist card to start listening.

---

## 🌐 Deploy to GitHub Pages

1. Push your `index.html` and `README.md` to your GitHub repository root.
2. In your repository, go to **Settings** > **Pages** (in the left sidebar).
3. Under **Build and deployment > Branch**, choose:
   - Branch: `main` (or `master`)
   - Folder: `/ (root)`
4. Click **Save**.
5. Your application will be live at:
   ```text
   https://<your-username>.github.io/<your-repo-name>/
   ```

---

## 📄 License
This project is open-source and free to use for educational and personal projects.
