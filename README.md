<div align="center">

<img src="./assets/speakout-v8.3.4-cinematic.gif" width="100%" alt="Speakout v8.3.4 cinematic demo">

# SPEAKOUT

### Speak. Think. Type.

**Private, system-wide voice intelligence for macOS, Windows and Linux.**

Hold one key. Speak naturally. Release.  
Speakout turns your voice into clean text or structured prompts while keeping the core voice workflow local.

[![Version](https://img.shields.io/badge/version-8.3.4%20Stable-111111?style=for-the-badge)](#)
[![Tests](https://img.shields.io/badge/tests-171%20%2F%20171-111111?style=for-the-badge)](#)
[![Telemetry](https://img.shields.io/badge/telemetry-none-111111?style=for-the-badge)](#)
[![Platforms](https://img.shields.io/badge/macOS%20·%20Windows%20·%20Linux-supported-111111?style=for-the-badge)](#)

[**Launch Interactive Demo**](https://codesource18.github.io/speakout-downloads/) ·
[**Download**](#download) ·
[**How it works**](#how-it-works) ·
[**Setup**](#platform-setup)

</div>

---

## A README that behaves like the product

The animated hero above works directly in GitHub.

The companion GitHub Pages experience is actually interactive:

**https://codesource18.github.io/speakout-downloads/**

Inside it, users can switch platform, click into a real typing field, hold the Speakout key, watch **Listening → Processing → Done**, see text inserted, browse the redesigned **History** cards, explore **Prompt Intelligence**, simulate updates, and open the new **Contact** portal.

> GitHub README pages block arbitrary JavaScript, so the truly interactive controls live in GitHub Pages while the README remains fast and native to GitHub.

---

<a id="how-it-works"></a>

## How it works

```text
HOTKEY
  ↓
MICROPHONE CAPTURE
  ↓
LOCAL SPEECH ENGINE
  ↓
INTENT DETECTION
  ↓
PLAIN TEXT OR PROFESSIONAL PROMPT FRAMEWORK
  ↓
FINAL CLEANUP
  ↓
TEXT INSERTION
  ↓
DONE
```

The current audited release is **Speakout 8.3.4 Stable** with **171 passed / 0 failed / 0 skipped** automated tests.

The active Apple Silicon speech path uses local `whisper.cpp` FP16 Metal bindings. The audit reports a **sub-2-second latency envelope** and **<110 MB runtime footprint** on the audited Apple Silicon configurations.

---

## Prompt Intelligence

Speakout does not force every sentence into a giant prompt.

Short input can stay plain. Complex instructions can be organized using:

```text
ROLE
  ↓
CONTEXT
  ↓
TASK
  ↓
REQUIREMENTS
  ↓
CONSTRAINTS
  ↓
FORMAT
```

The current audit also identifies **≤2-line plain-text passthrough**, so short dictation is not unnecessarily over-processed.

---

## New in 8.3.4

### Monochrome B&W interface
A quieter black-and-white product language with less visual noise.

### Numbered History cards
Recent work is easier to scan:

```text
01  Launch page prompt          Prompt
02  Follow-up message           Message
03  Product specification       Structured Task
```

### Update persistence
Update state now survives relaunches correctly.

### Prompt-engine refinements
Professional Prompt Framework + short-form passthrough behavior.

### Contact portal
Support/contact is now part of the product flow.

---

<a id="platform-setup"></a>

# Platform setup

<details open>
<summary><strong>macOS — Apple Silicon</strong></summary>

<br>

[**Download Speakout for macOS (.dmg) →**](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.4/Speakout-v8.3.4-apple-silicon.dmg)

Install Speakout, complete the first-run setup, then grant the permissions requested by the current build.

Typical macOS operation involves:
- Microphone
- Accessibility
- Input Monitoring

Use **Open Privacy Settings** inside Speakout whenever the setup guide asks for a permission.

Then:

```text
Hold FN → Speak → Release FN
                ↓
     Listening → Processing → Done
```

</details>

<details>
<summary><strong>Windows 10 / 11 — 64-bit</strong></summary>

<br>

- [**Download Windows Installer (.msi) →**](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.4/Speakout-v8.3.4-windows-x64.msi)
- [**Download Windows Portable (.zip) →**](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.4/Speakout-v8.3.4-windows-x64.zip)

Complete the microphone/system-input setup shown by Speakout.

```text
Hold Control → Speak → Release
                    ↓
             Processing → Done
```

</details>

<details>
<summary><strong>Linux — x86_64</strong></summary>

<br>

- [**Download Linux Universal (.AppImage) →**](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.4/Speakout-v8.3.4-linux-x86_64.AppImage)
- [**Download Linux Debian / Ubuntu (.deb) →**](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.4/Speakout-v8.3.4-linux-amd64.deb)

Install the package and follow the platform setup in Speakout.

Linux global-hotkey and text-injection behavior can vary between desktop environments, especially X11 and Wayland.

</details>

---

## HUD states

**LISTENING** — voice capture is active.  
**PROCESSING** — Speakout is finalizing the text.  
**DONE** — text has been inserted.  
**ERROR** — a real failure is surfaced instead of silently pretending success.

---

## Local-first privacy

The audited architecture reports:
- local speech processing
- local prompt processing
- local application data
- zero telemetry
- no exposed tokens

Speakout also includes an update system, so update checks/downloads can use the network. This README therefore says **local-first voice processing** rather than implying the app never makes any network request.

---

## Updates

Speakout 8.3.4 uses a dual-layer update architecture:

```text
version metadata + atomic package replacement
                    +
     tauri updater + signed verification
```

The current audit also confirms update-persistence fixes.

---

## Performance

| Metric | Audited result |
|---|---:|
| Tests | **171 passed** |
| Failed | **0** |
| Skipped | **0** |
| Post-speech latency | **Sub-2s audited envelope** |
| Runtime footprint | **<110 MB** |
| Apple acceleration | **Metal** |
| Speech engine | **whisper.cpp FP16 Metal bindings** |

Actual performance varies by machine, recording length, mode and platform.

---

<a id="download"></a>

# Download

<div align="center">

| Platform | Format | Direct Download |
|:---|:---|:---:|
| **macOS (Apple Silicon)** | `.dmg` Installer | [**Download DMG (5.2 MB) →**](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.4/Speakout-v8.3.4-apple-silicon.dmg) |
| **Windows 10 / 11 (x64)** | `.msi` Windows Installer | [**Download MSI →**](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.4/Speakout-v8.3.4-windows-x64.msi) |
| **Windows 10 / 11 (x64)** | `.zip` Portable Package | [**Download ZIP →**](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.4/Speakout-v8.3.4-windows-x64.zip) |
| **Linux (Universal)** | `.AppImage` Executable | [**Download AppImage →**](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.4/Speakout-v8.3.4-linux-x86_64.AppImage) |
| **Linux (Debian / Ubuntu)** | `.deb` Package | [**Download DEB →**](https://github.com/codesource18/speakout-downloads/releases/download/v8.3.4/Speakout-v8.3.4-linux-amd64.deb) |

</div>

---

## Interactive demo deployment

This package contains:

```text
README.md
assets/
└── speakout-v8.3.4-cinematic.gif

docs/
└── index.html
```

Enable:

```text
GitHub → Settings → Pages → Deploy from branch → main → /docs
```

Expected URL:

```text
https://codesource18.github.io/speakout-downloads/
```

> Browser note: the physical macOS FN/Globe key is not reliably exposed to normal JavaScript. The web demo therefore provides a real press-and-hold FN control on screen and an `F` keyboard simulation. Windows/Linux demo mode supports `Control`.

---

<div align="center">

# Speak. Think. Type.

**Speakout disappears into your workflow so your ideas don't have to.**

[**Launch Interactive Demo**](https://codesource18.github.io/speakout-downloads/) ·
[**Download Speakout**](https://github.com/codesource18/speakout-downloads/releases/latest)

`8.3.4 Stable` · `171 / 171 tests` · `Local-first` · `macOS · Windows · Linux`

</div>
