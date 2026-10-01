# Speakout

### Speak naturally. Type anywhere.

Speakout is a lightweight macOS voice-dictation app designed to turn speech into text quickly while keeping core transcription processing local on your Mac.

Hold the **Fn key**, speak naturally, release the key, and Speakout processes and inserts your text into the active application.

---

## Latest Version

**Speakout v0.7.0 Beta**

- **Target Architecture:** Apple Silicon Macs — M1 / M2 / M3 / M4
- **Target OS:** macOS 12.0 or later
- **Empirically Tested:** MacBook Air M2 running macOS 15.1 Sequoia

---

# Download Speakout

### [⬇️ Download Speakout v0.7.0 Beta (.dmg)](https://github.com/codesource18/speakout-downloads/raw/refs/heads/main/Speakout-v0.7.0-beta-apple-silicon.dmg)

| Property | Details |
| :--- | :--- |
| **File** | `Speakout-v0.7.0-beta-apple-silicon.dmg` |
| **Version** | `0.7.0 Beta` |
| **Architecture** | `Apple Silicon arm64` |
| **Size** | `4.6 MB` (4,855,267 bytes) |
| **SHA-256** | `6975e2509b896157392d51d18be2d7723a90bc7757a7063e666515fd7657ca48` |

---

## Installation

1. Download the DMG above.
2. Open `Speakout-v0.7.0-beta-apple-silicon.dmg`.
3. Drag **Speakout** into your **Applications** folder.
4. Launch Speakout from Applications or Spotlight.
5. Grant Microphone and Accessibility permissions when prompted.
6. Complete the in-app speech model setup wizard.
7. Hold **Fn** and start speaking.
8. Release **Fn** and Speakout inserts your text at your cursor.

---

## How Speakout Works

- **Hold Fn**: Speakout begins listening immediately.
- **Speak**: Talk naturally.
- **Release Fn**: Speakout processes your speech on-device.
- **Done**: Your text is instantly inserted into the application you are using.

---

## Features

- **Hold-Fn push-to-talk dictation**
- **Local Whisper speech recognition**
- **Apple Silicon Metal GPU acceleration**
- **Fast post-speech processing**
- **Automatic punctuation and capitalization**
- **Filler-word cleanup** (*"um"*, *"uh"*)
- **Spoken list formatting** (bulleted and numbered lists)
- **Intent-aware formatting**
- **Personal dictionary support**
- **Dictation history & search**
- **Session statistics**
- **Floating Listening / Processing / Done HUD**
- **Local-first processing**
- **No Homebrew required**
- **No Terminal required for normal dictation setup**

---

## Prompt Intelligence

Speakout includes built-in local deterministic intelligence for:
- Dictation cleanup
- Intent detection
- Punctuation & capitalization
- Filler removal
- List formatting
- Structured text formatting

Optional generative LLM polishing currently supports a user-managed local Ollama installation (`http://127.0.0.1:11434`).

> [!NOTE]
> **Ollama is NOT required** for normal Speakout dictation. Core transcription and fast-path formatting run 100% locally out of the box.

---

## Privacy

Core speech transcription runs locally on your Mac.

Speakout does not require uploading your microphone audio to a remote transcription service for normal dictation.

Downloaded speech models and update checks may require an internet connection.

---

## Beta Notice

Speakout v0.7.0 is currently a **free beta**.

This build is not currently distributed using a paid Apple Developer ID certificate and is not Apple-notarized. Because of this, macOS may display standard first-launch security warnings.

No Gatekeeper, SIP, quarantine, or macOS security protections are automatically bypassed by Speakout.

---

## Compatibility

- **Current Target:** macOS 12.0+ on Apple Silicon (`arm64`)
- **Empirically Tested:** MacBook Air M2 / macOS 15.1
- **Declared Target Scope:** M1, M2, M3, and M4 are part of the declared Apple Silicon target (*M2 was the primary hardware validation platform in this session*). Intel Macs are not currently advertised as supported.

---

## Current Version

- **Release:** Speakout v0.7.0 Beta
- **Build:** Apple Silicon `arm64`

---

## Feedback & Support

Speakout is currently being tested with a beta group. If you experience:
- Installation problems
- Microphone issues
- Accessibility permission problems
- Missing words or incorrect formatting
- Crashes or slow processing

Please open an issue on the [Issue Tracker](https://github.com/codesource18/speakout-downloads/issues) with your Mac model, macOS version, and reproduction steps.

---

### Speakout
*Voice to text. Fast. Local. Simple.*
