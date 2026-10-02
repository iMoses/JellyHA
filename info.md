# JellyHA — Jellyfin for Home Assistant

**v1.5.3** · [Full Changelog](https://github.com/zupancicmarko/JellyHA/blob/main/CHANGELOG.md) · [Documentation](https://github.com/zupancicmarko/JellyHA/tree/main/docs)

![JellyHA Library Card](https://github.com/zupancicmarko/JellyHA/raw/main/docs/JellyHA-Library-Grid.png)

JellyHA integrates your Jellyfin media server directly into Home Assistant with a full-featured Lovelace card, rich media player entities, and powerful automation sensors.

---

### 🆕 What's new in v1.5.3

- 📺 **Android TV & Fire TV Device Session Matching** — Resolved an issue where Android TV, Google TV, and Fire TV clients remained permanently `idle` due to Jellyfin assigning database row IDs instead of hardware client IDs; added name-based fallback matching (fixes #27, PR #52).
- 🎮 **Reliable Remote Control Routing** — Remote playback commands now target the active session's client device ID directly.
- 🎞️ **Enriched Playback Stream Metadata** — Automatically populates video dimensions, aspect ratio, HDR dynamic range, and local `file_path` attributes across both media players and sensors.
- 🛡️ **Hassfest Compliance** — Cleaned up integration manifest requirements to align with Home Assistant core standards.

---

### ✨ Features

- 🎬 **Library Card** — Browse movies & shows in Carousel, Grid, or List view with Next Up support
- ⏯️ **Full Playback Control** — Play, pause, stop, seek, shuffle, repeat, volume via `media_player` entities
- 📡 **Chromecast** — Cast with subtitle burn-in and language selection
- 🔍 **Search Service** — Filter by genre, studio, person, and more
- 📊 **Rich Sensors** — Library stats, storage, transcoding streams, connected clients, latest media
- 🤖 **Automation-Ready** — Device triggers, segment events, chapter events, HDR detection
- 🌐 **Multi-Instance** — Multiple Jellyfin servers in one HA instance
- 🃏 **Community Card Compatible** — Works with Mini Media Player, Mushroom, Universal Media Player

---

### 📦 Installation

1. Install via HACS.
2. **Restart Home Assistant**.
3. Go to **Settings → Devices & Services → Add Integration → JellyHA**.
4. Add the Lovelace resource:
   - **URL**: `/jellyha/jellyha-cards.js`
   - **Type**: JavaScript Module

[📖 Full documentation](https://github.com/zupancicmarko/JellyHA/tree/main/docs) · [💬 Community](https://github.com/zupancicmarko/JellyHA/discussions) · [🐛 Issues](https://github.com/zupancicmarko/JellyHA/issues)
