# Speakout v8.3.1 — Local Voice Dictation & Prompt Intelligence for Apple Silicon

Speakout v8.3.1 is an ultra-fast, local-first, Metal GPU-accelerated voice dictation and prompt intelligence platform for macOS.

[![Latest Release](https://img.shields.io/badge/Release-v8.3.1_Stable-blue.svg)](https://github.com/codesource18/speakout-downloads/releases/tag/v8.3.1)
[![Architecture](https://img.shields.io/badge/Architecture-Apple_Silicon_(arm64)-orange.svg)](https://github.com/codesource18/speakout-downloads)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📦 Direct Download

- **[Speakout-v8.3.1-apple-silicon.dmg](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.1/Speakout-v8.3.1-apple-silicon.dmg)** (5.08 MB)
- **Architecture**: Apple Silicon (M1 / M2 / M3 / M4)
- **macOS Compatibility**: macOS 12 Monterey or higher (Optimized for macOS 15 Sequoia)
- **RAM Footprint**: < 120 MB (0 external server dependencies, 0 RAM bloat)

---

## ⚡ What's New in v8.3.1

- **Liquid Glass Voice HUD**: Golden mic listening animation, orbit loader processing, and gold checkmark paste.
- **Background Resident Tray Mode**: When closing the dashboard window, Speakout stays alive in the macOS menu bar tray. Pressing Fn anywhere immediately activates voice dictation.
- **Prompt Intelligence Engine**: Multi-step idea structuring, mid-sentence voice corrections (*"actually"*, *"scratch that"*), and spoken snippets.
- **Apple Silicon Metal Compute**: 3x faster local inference powered directly by Metal GPU compute.
- **100% Local-First & Zero Telemetry**: Air-gapped, zero cloud egress, 100% private.

---

## 🚀 First-Run Installation (macOS Gatekeeper)

1. Drag `Speakout.app` to your `/Applications` folder.
2. Run the quick one-time terminal unlock:
   ```bash
   xattr -cr /Applications/Speakout.app && open /Applications/Speakout.app
   ```
   *Or go to **System Settings > Privacy & Security > Security** and click **Open Anyway**.*
