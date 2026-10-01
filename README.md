<p align="center">
  <img src="assets/speakout-hero-cinematic.webp" width="100%" alt="Speakout for macOS" style="border-radius: 16px; box-shadow: 0 20px 50px rgba(0,0,0,0.5);">
</p>

<br>

<h1 align="center">Speakout</h1>

<p align="center">
  <strong>Speak naturally. Type anywhere.</strong>
</p>

<p align="center">
  <em>High-performance, local voice dictation engineered exclusively for Apple Silicon.</em>
</p>

<p align="center">
  <strong>Hold Fn · Speak · Release · Done</strong>
</p>

<p align="center">
  <a href="https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v0.7.0-beta-apple-silicon.dmg"><img src="https://img.shields.io/badge/Release-v0.7.0%20Beta-f59e0b?style=for-the-badge&logo=apple&logoColor=white" alt="v0.7.0 Beta"></a>
  <img src="https://img.shields.io/badge/Platform-macOS%2012.0%2B-black?style=for-the-badge&logo=apple&logoColor=white" alt="macOS 12+">
  <img src="https://img.shields.io/badge/Architecture-Apple%20Silicon%20(arm64)-1e293b?style=for-the-badge" alt="Apple Silicon">
  <img src="https://img.shields.io/badge/Engine-Local%20Whisper%20Metal-10b981?style=for-the-badge" alt="Metal GPU">
  <img src="https://img.shields.io/badge/Privacy-Zero%20Audio%20Uploads-3b82f6?style=for-the-badge" alt="100% Local">
</p>

---

<br>

# Download Speakout

### **Speakout v0.7.0 Beta for Apple Silicon**
Universal Native Build for **M1 · M2 · M3 · M4**

<p align="center">
  <a href="https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v0.7.0-beta-apple-silicon.dmg">
    <img src="https://img.shields.io/badge/%E2%AC07%EF%B8%8F%20Download%20Speakout%20v0.7.0%20Beta%20(.dmg)-f59e0b?style=for-the-badge&labelColor=181b26&color=f59e0b" height="48" alt="Download Speakout for macOS">
  </a>
</p>

<div align="center">

| Specification | Target Details |
| :--- | :--- |
| **Package File** | [`Speakout-v0.7.0-beta-apple-silicon.dmg`](https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v0.7.0-beta-apple-silicon.dmg) |
| **Version** | `0.7.0 Beta (Production-Sealed Bundle)` |
| **Architecture** | Apple Silicon (`arm64`) |
| **Package Size** | `5.28 MB` (5,276,123 bytes) |
| **Hardware Target** | Apple Silicon Macs (M1 / M2 / M3 / M4) · macOS 12.0+ |
| **Empirical Test Environment** | MacBook Air M2 / macOS 15.1 Sequoia |
| **SHA-256 Checksum** | `68730479995af8c51f72333fe68f8dbb44160d4d7affabbeb2714343040fc498` |

</div>

---

<br>

# Voice → text without breaking your flow.

Hold **Fn**. Speak naturally. Release.

Speakout cleans up your words, removes fillers, applies grammar and intent, and places the formatted text directly at your active cursor.

<p align="center">
  <img src="assets/speakout-live-demo.gif" width="100%" alt="Speakout Live Dictation Demo" style="border-radius: 12px; border: 1px solid #282f44;">
</p>

---

<br>

# Meet Speakout.

### *One place for everything you say.*

<p align="center">
  <img src="assets/speakout-ui-showcase.webp" width="100%" alt="Speakout UI Suite" style="border-radius: 14px;">
</p>

### The 5 Native Hubs:

* **🏠 Home / Dashboard** — Live dictation metrics, real-time Metal GPU health, and your latest session activity.
* **📜 History** — Instant, searchable archive of your previous dictations, word counts, and execution timestamps.
* **🧠 Prompt Intelligence** — Deterministic speech intelligence that formats spoken bullet points, numbered lists, and emails instantly.
* **⚙️ Settings** — Custom push-to-talk hotkeys, personal dictionary terms, and microphone calibration.
* **✨ In-App Updates** — One-click release verification and updates without external dependencies.

---

<br>

# It feels instant.

<p align="center">
  <img src="assets/speakout-hud-demo.gif" width="540" alt="Speakout Floating HUD" style="border-radius: 28px; border: 1px solid rgba(245,158,11,0.3);">
</p>

<table width="100%" style="border: none;">
  <tr>
    <td width="25%" valign="top">
      <h3>01 · Hold</h3>
      <p>Hold the <strong>Fn key</strong>. Speakout's floating golden HUD activates immediately with zero cold-start delay.</p>
    </td>
    <td width="25%" valign="top">
      <h3>02 · Speak</h3>
      <p>Speak naturally at normal speed. The audio wave visualizer tracks your voice in uncompressed 16kHz audio.</p>
    </td>
    <td width="25%" valign="top">
      <h3>03 · Release</h3>
      <p>Release the key. The on-device Whisper Metal engine processes speech with sub-second latency.</p>
    </td>
    <td width="25%" valign="top">
      <h3>04 · Done</h3>
      <p>Clean, formatted text is injected right into your target app (Slack, Notion, VS Code, Notes, Browser).</p>
    </td>
  </tr>
</table>

---

<br>

# Built to disappear.

Speakout runs locally with Apple Silicon Metal acceleration, delivering near-instant transcription speed without draining battery life or sending audio to third-party servers.

```
┌────────────────────────────────────────────────────────────────────────┐
│                   ENGINE PIPELINE BENCHMARK (M2)                       │
├───────────────────────────────┬───────────────────┬────────────────────┤
│ Speech Duration               │ Median Latency    │ P95 Latency        │
├───────────────────────────────┼───────────────────┼────────────────────┤
│ 5s Speech Sample              │ 341 ms            │ 388 ms             │
│ 15s Speech Sample             │ 525 ms            │ 590 ms             │
│ 30s Speech Sample             │ 512 ms            │ 574 ms             │
│ 60s Extended Dictation        │ 1.03 s            │ 1.18 s             │
└───────────────────────────────┴───────────────────┴────────────────────┘
```
*Empirically measured engine-pipeline benchmarks on MacBook Air M2 (8GB Unified Memory, macOS 15.1).*

---

<br>

# From voice to text.

A local-first pipeline built to stay completely out of your way.

<p align="center">
  <img src="assets/speakout-voice-pipeline.svg" width="100%" alt="Speakout Voice Pipeline Architecture">
</p>

---

<br>

# Features

<table width="100%">
  <tr>
    <td width="50%" valign="top">
      <h4>🎙️ Push-to-Talk Precision</h4>
      <p>Hold Fn to dictate, release to insert. No wake-words, no background eavesdropping, no accidental triggers.</p>
    </td>
    <td width="50%" valign="top">
      <h4>⚡ Metal GPU Acceleration</h4>
      <p>Direct Apple Silicon Metal kernel bindings for Whisper. Transcribes speech in ~340ms.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4>🧠 Prompt Intelligence</h4>
      <p>Deterministic local formatting for spoken lists, bullet points, emails, and automatic punctuation.</p>
    </td>
    <td width="50%" valign="top">
      <h4>🔒 100% Local First</h4>
      <p>Microphone audio never leaves your Mac for core dictation. Zero telemetry on your voice data.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4>📖 Personal Dictionary</h4>
      <p>Teach Speakout technical acronyms, team jargon, names, or custom terminology.</p>
    </td>
    <td width="50%" valign="top">
      <h4>🪶 Ultra-Lightweight</h4>
      <p>Native Rust &amp; Tauri architecture. Self-contained 5.2 MB package with zero Homebrew or terminal dependencies.</p>
    </td>
  </tr>
</table>

---

<br>

# Get started in 60 seconds.

1. **[Download the DMG](https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v0.7.0-beta-apple-silicon.dmg)**.
2. Open `Speakout-v0.7.0-beta-apple-silicon.dmg`.
3. Drag **Speakout** into your **Applications** folder.
4. Launch Speakout. *(On first launch, if prompted, select **Open** in System Settings → Privacy & Security).*
5. Grant Microphone & Accessibility permissions.
6. Hold **Fn** and begin speaking into any app.

**That's it.**

---

<br>

# Ready to stop typing?

<p align="center">
  <a href="https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v0.7.0-beta-apple-silicon.dmg">
    <img src="https://img.shields.io/badge/%E2%AC07%EF%B8%8F%20Download%20Speakout%20v0.7.0%20Beta-f59e0b?style=for-the-badge&labelColor=181b26&color=f59e0b" height="48" alt="Download Speakout for macOS">
  </a>
</p>

<p align="center">
  <strong>Apple Silicon Native · macOS 12.0+ · Free Beta</strong>
</p>

---

<br>

<details>
<summary><strong>Technical Specifications &amp; Release Notes (Click to expand)</strong></summary>

<br>

### Architecture & System Details
* **Target Architecture**: macOS Apple Silicon (`arm64`)
* **Declared Scope**: M1, M2, M3, M4 Macs
* **Minimum OS**: macOS 12.0 Monterey or later
* **Runtime**: Native Rust engine with Metal GPU shader execution
* **GUI Shell**: Frosted liquid-glass Tauri v2 interface

### Verification Hashes
* **File**: `Speakout-v0.7.0-beta-apple-silicon.dmg`
* **Size**: `5,276,123` bytes
* **SHA-256**: `68730479995af8c51f72333fe68f8dbb44160d4d7affabbeb2714343040fc498`
* **Image Checksum**: `hdiutil verify: VALID`

### Free Beta Distribution Notice
* Speakout v0.7.0 is a free testing/beta release.
* This build is ad-hoc signed with verified macOS entitlements and sealed bundle integrity.
* No macOS security bypasses (`xattr`, quarantine stripping, SIP tampering) are used.

</details>

---

<br>

<p align="center">
  <sub><strong>Speakout</strong> · Voice to text. Fast. Local. Simple.</sub><br>
  <sub>Maintained by <a href="https://github.com/codesource18"><strong>codesource18</strong></a></sub>
</p>
