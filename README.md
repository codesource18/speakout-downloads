# Speakout — Open-Source Voice Dictation for Apple Silicon

Speakout is a blazingly fast, privacy-first, Metal-accelerated local voice intelligence system for macOS.

[![Latest Release](https://img.shields.io/badge/Release-v0.9.0_Beta-blue.svg)](https://github.com/codesource18/speakout-downloads/releases/tag/v0.9.0)
[![Architecture](https://img.shields.io/badge/Architecture-Apple_Silicon_(arm64)-orange.svg)](https://github.com/codesource18/speakout-downloads)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## Direct Download

- **[Speakout-v0.9.0-apple-silicon.dmg](https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v0.9.0-apple-silicon.dmg)** (5.09 MB)
- **SHA-256**: `882263b6357a0ba9ed77cd79114a37c988b950786e231159d709bab28d007023`
- **Architecture**: Apple Silicon (M1 / M2 / M3 / M4)
- **macOS Version**: macOS 12 Monterey or higher (Optimized for macOS 15 Sequoia)

---

## What's New in Speakout v0.9.0 Beta (Voice Engine v2)

- **Voice Engine v2 Architecture**: Streaming partial decoding during Fn hold with fast tail-only finalization upon key release.
- **Zero First/Last Word Clipping**: Pre-warmed rolling audio pre-buffer (100–300 ms) and CoreAudio trailing audio flush (35 ms).
- **Realtime VAD**: Adaptive energy and zero-crossing rate voice activity detection.
- **Indian English & Multilingual Priming**: Built-in acoustic and vocabulary priming for Indian English (₹, rupees, lakh, crore, tech terms) and multilingual speech (Telugu, Hindi, Kannada, Tamil).
- **Deterministic Cleanup Engine v2**: Ultra-fast (<1 ms) filler removal, stutter deduplication, and currency normalization with dual raw/clean transcript preservation.
- **Genuine Prompt Engineer IR**: Intermediate representation (`PromptIdea`) converting spoken thoughts into structured prompts without hallucinating unmentioned tools.
- **100% Local-First & Private**: Zero external cloud calls, zero Ollama dependency for normal dictation.

---

## First-Run Installation (3 Clicks)

Because Speakout is an independent open-source application and not distributed via the Mac App Store, macOS Gatekeeper requires a one-time approval on first launch:

1. **Open & Click "Done"**: Drag Speakout to Applications and double-click to open. When macOS displays *"Apple could not verify Speakout is free of malware"*, click **Done**.
2. **Open System Settings**: Go to ** > System Settings > Privacy & Security**, and scroll down to the **Security** section.
3. **Click "Open Anyway"**: Next to *"Speakout was blocked to protect your Mac"*, click **Open Anyway**, authenticate with Touch ID or password, and click **Open**.

> **Note**: You only do this once! All subsequent in-app updates install automatically with zero prompts.

---

## Verification & Integrity

```bash
# Verify download SHA-256
shasum -a 256 Speakout-v0.9.0-apple-silicon.dmg

# Verify inside-out ad-hoc signature & entitlements
codesign --verify --deep --strict --verbose=2 /Applications/Speakout.app
codesign -d --entitlements :- /Applications/Speakout.app
```
