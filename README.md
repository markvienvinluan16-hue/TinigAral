# TinigAral

**TinigAral** (*Tinig* = voice + *Aral* = learn/study) is a modern Android podcast and audio-learning player designed for Filipino learners listening to AI-curated educational episodes in a warm Taglish experience. Built with Kotlin, Jetpack Compose, Material Design 3, and Media3 ExoPlayer, it combines flagship audio engineering with offline-first reliability and a Warm Editorial Dark interface.

---

## Why TinigAral?

TinigAral turns everyday moments into effortless learning sessions—whether you are commuting, walking, or taking a quiet break:

- **Bite-sized learning sa biyahe o pahinga** — Absorb lessons cleanly on the go without needing to stare at a screen.
- **Skill upskilling at career or study growth** — Organize study episodes, topics, and hosts into focused listening queues.
- **Screen-free daily curiosity via AI podcasts** — Relaxed, distraction-free audio journalism aesthetic with optional reactive audio visuals.
- **Consistent habits gamit ang offline study lists** — Pin episodes for offline listening, manage smart cache limits, and back up your study playlists locally.

---

## Features

### Audio & Playback Engine
- **Gapless Playback & Configurable Crossfade**: Smooth `0s` (Gapless) up to `12s` equal-power crossfade transitions orchestrated across dual `ExoPlayer` instances with seamless `MediaSession` handoff.
- **Real-Time Adaptive Loudness Normalization**: Measures PCM audio levels dynamically and adjusts gain toward selectable targets—**Quiet (-18 LUFS)**, **Balanced (-14 LUFS)**, or **Punchy (-11 LUFS)**—using `LoudnessEnhancer`, peak headroom limiting, and persistent per-episode loudness caching.
- **5-Band Equalizer & Speed Controls**: Built-in hardware equalizer presets and custom band sliders, playback speeds from `0.75x` to `2.0x`, skip silence, and a **Sleep Timer** (`15m`, `30m`, `45m`, `60m`, or *End of Episode*).
- **Now Playing Studio**: Full-bleed Album Art Hero with an optional toggleable reactive **Audio Orb** visualizer and embedded audio-file cover art extraction.

### Daily Listening UX
- **Swipe Gestures**: Swipe left/right on the floating mini-player or Now Playing artwork to skip episodes, and swipe up on the mini-player to expand Now Playing.
- **Home Screen Playback Widget**: Native `AppWidgetProvider` displaying current episode title, host/format metadata, rounded cover artwork, and Play/Pause/Previous/Next controls, with one-tap widget pinning from Settings.
- **Modern Taglish Copy & Warm Editorial Dark Theme**: Styled with deep warm charcoal surfaces (`#0D0C0C` / `#171515`), Editorial Rose (`#FA3C52`) accents, and locally bundled `Plus Jakarta Sans` + `Inter` typography (with tabular timestamps).

### Library, Folders & Offline First
- **Cloud Folder Sync**: Streams and indexes audio files from a cloud hierarchy via a lightweight Google  endpoint.
- **Smart Browsing**: Recent playback artwork carousel, tag & host filter chips, search, sort orders, multi-select batch actions, and nested folder browsing with breadcrumbs.
- **Offline Cache & Study Playlists**: One-tap offline pinning, automatic smart caching with configurable storage cap, full Offline Mode toggle, and JSON playlist/metadata export & import.
- **Zero-Permission Media & Support Flow**: Includes an **About TinigAral** section in Settings with a **Buy Me a Cup of Coffee** modal displaying **Vien Vi**'s GCash InstaPay QR code plus zero-permission **Save QR to Photos** (`MediaStore` / SAF) and **Share QR** (`FileProvider`).



## Developer & Support

- **Developer**: **Vien Vi**
- **Contact**: `vienx1998@gmail.com`

If TinigAral helps your daily commute or study routine, you can support ongoing development directly inside the app via **Settings → About TinigAral → Buy Me a Cup of Coffee** (GCash InstaPay QR).
