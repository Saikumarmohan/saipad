# ⌨️ SaiPad — 4x4 Mechanical Macropad & Developer Console

An advanced, corporate-safe programmable 4x4 mechanical macropad powered by the **Waveshare RP2040-Zero**.

[![Live Studio](https://img.shields.io/badge/Live%20Studio-saikumarmohan.github.io%2Fsaipad-blue?style=for-the-badge&logo=googlechrome)](https://saikumarmohan.github.io/saipad/)
[![MCU](https://img.shields.io/badge/MCU-RP2040--Zero-blue?style=for-the-badge)](https://www.raspberrypi.com/documentation/microcontrollers/rp2040.html)
[![Version](https://img.shields.io/badge/Release-v1.5.1-brightgreen?style=for-the-badge)](releases/4x4keyboard_rp2040_zero_v1.5.1.uf2)
[![EDR Safe](https://img.shields.io/badge/Corporate%20Safe-CrowdStrike%20%7C%20Defender%20Clean-success?style=for-the-badge)](https://saikumarmohan.github.io/saipad/)
[![License](https://img.shields.io/badge/License-MIT-orange?style=for-the-badge)](LICENSE)

---

## 🌟 What is SaiPad?

**SaiPad** is a customizable 16-key tactile macro deck designed for developers, creators, streamers, and power users who need instant one-tap control without installing bloatware or background daemons.

👉 **Launch Live Web Studio:** **[https://saikumarmohan.github.io/saipad/](https://saikumarmohan.github.io/saipad/)**

### 💡 Why SaiPad is Different:
* **Zero Drivers, Zero Native Bloatware:** Operates as a standard USB HID Keyboard + Mouse. 100% plug-and-play across Windows, macOS, and Linux.
* **100% Corporate IT & EDR Safe:** Safe against CrowdStrike, Microsoft Defender, and SentinelOne. No suspicious `.exe` installers; all customization runs client-side in Google Chrome or Microsoft Edge via native **WebSerial**.
* **Onboard Flash EEPROM Persistence:** Mappings, hold times, and per-profile RGB colors save directly to the RP2040's internal flash memory in 1 millisecond. Unplugging the cable or rebooting your PC never loses your configuration.

---

## 🚀 Key Features

### 1. 🌐 Zero-Installation Web Studio ([Launch Studio](https://saikumarmohan.github.io/saipad/))
* **⚡ Zero-Click Auto-Reconnect:** Remembers paired devices and automatically connects when the page loads or when the USB cable is plugged in.
* **📱 PWA Desktop App:** Install directly as a standalone desktop app from Chrome/Edge (no browser URL bar, pins to Windows taskbar).
* **⌨️ VIA-Style Keycode Palette:** Click any key on the visual 4x4 matrix, then 1-click assign from a categorized palette (Basic, Media, Git/Dev, Windows, Scripts, Actions).
* **📚 Curated 110+ Preset Library:** Real-time search and filter across 110+ production-grade profiles dynamically loaded from GitHub:
  * 👨‍💻 **Developer & Git:** Git Master, VS Code Supercharged, Docker, Kubernetes, Linux Bash, Python Data Notebook, C++, Rust Cargo, Go, Next.js.
  * 🎨 **Creative & Design:** Figma UI/UX, Blender 3D, Blender Sculpt, Photoshop Essentials, Illustrator Vector, After Effects, Cinema 4D, Canva.
  * 🎬 **Video & Audio:** Premiere Pro, DaVinci Resolve Studio, Ableton Live 12, FL Studio 21, Logic Pro, Pro Tools, Reaper, Audacity, Virtual DJ.
  * 🎙️ **Streaming & Comms:** OBS Studio, Streamlabs, Discord Stream, Camera Switcher, Soundboard Trigger, Zoom & Teams Meetings, YouTube Live.
  * 📊 **Office & Finance:** Excel Financial Pro, Google Sheets, Notion PKM, Obsidian Markdown, PowerPoint Remote, QuickBooks Invoicing.
  * 🎮 **Gaming & Esports:** CS2 / Valorant Tactical, Flight Sim MSFS, Racing Rig, MMO Action, MOBA LoL/Dota, Minecraft Builder.
  * 🤖 **AI & Data Science:** AI Prompt Engineer, Midjourney Prompter, Ollama Local LLM, ComfyUI Nodes, PyTorch Deep Learning, Pandas Wrangling.
  * ⚡ **System & Scripts:** Windows PowerToys, Windows SysAdmin Pro, Network IT Diagnostic, CRT Terminal, Backup Disk Maintenance.
* **🛠️ Interactive Preset Generator & Layout Builder:** Visually build custom 16-key profiles for any software, customize individual key action types (Char, Special Keycode, Modifier Shortcut, String Macro, Action, Win+R Script Launcher), test in real-time, clone from your active profile, use quick starter templates (Dev, Numpad, Gaming, Media), and export `.json` or flash directly to the keyboard.
* **🤖 Supercharged AI Copilot:** 1-Click app selectors for popular tools (Blender, Photoshop, Premiere, Resolve, VS Code, Ableton, FL Studio, Figma, Excel, Discord, CS2, AutoCAD, Midjourney, Docker, TradingView), auto-prompt generation, `.json` file upload / open, live syntax validation, and instant hardware flashing.
* **🔊 Procedural Switch Sound Synthesizer:** Realistic Web Audio API mechanical acoustics:
  * 💾 **IBM Model M (Buckling Spring)** with authentic metallic spring resonance ping!
  * 🔵 **Cherry MX Blue** (Crisp click)
  * 🔴 **Cherry MX Red** (Linear thock)
  * ⚓ **Kailh Box Navy** (Deep tactile click bar)
* **🧪 Hardware Matrix Continuity Tester:** Live diagnostics verifying physical switches, tracking scan latency (<5ms).
* **📜 Full JSON Drag-and-Drop:** Drop any `.json` layout anywhere in the browser to import, export single profiles or backup all 4 layers.
* **📟 Live Serial Protocol Monitor:** Real-time console inspecting raw TX/RX serial communication packets.

### 2. ⚡ USB Keystroke Script & Command Injection (`KT_SCRIPT = 5`)
* Uses Windows Run (`Win+R`) keystroke injection to launch applications, terminals, scripts, or URLs in 1 tap without installing software on the PC!
* Pre-built templates for `wt` (Windows Terminal), `code .` (VS Code), `calc` (Calculator), `explorer .`, `snippingtool`, `taskmgr`, `start https://chatgpt.com`, `start https://github.com`, and custom PowerShell one-liners (up to 63 characters).

### 3. 🛡️ Corporate Anti-Away (Stealth Jiggler)
* Moves the cursor ±1px every 45 seconds at the USB hardware level.
* Prevents Microsoft Teams, Slack, and your screen from going idle/away during long compilations, presentations, or reading sessions.
* Toggleable via the web dashboard or Key #13.

### 4. 🎨 3 Aesthetic Studio Themes
* **⚡ Pro Geek Mode:** High-tech dark theme with terminal commands, macros, git actions, and raw controls.
* **🏢 Corporate Mode:** Neutral, office-clean theme. Rebrands sensitive terms like "Jiggler" into legitimate features ("Presentation Stay-Awake").
* **💾 1990s Vintage Mechanical (Model M):** Authentic retro workstation beige chassis (`#dfd9ca`), 3D stepped PBT keycaps, classic monospace typography, and vintage status indicator panel.
* **🛡️ Emergency Boss Key:** One click on the shield button (or hitting `Esc`) swaps the screen to an innocent office calculator.

---

## ⚡ Profile Switching & Shortcuts

* **⏱️ Dual-Corner Hold (Key #13 + Key #16 for 2.0s):** Hold both bottom corner keys (#13 and #16) together for 2.0s to cycle profiles. Short taps fire normal key functions (avoids accidental switching during fast typing).
* **⚡ Directional Profile Switching (13 + 4 and 13 + 1):**
  * Hold **Key #13** (bottom-left) and tap **Key #4** (top-right) ➔ **Next Profile (Step Forward)**!
  * Hold **Key #13** (bottom-left) and tap **Key #1** (top-left) ➔ **Previous Profile (Step Backward)**!
* **🎯 Direct Profile Jump:** Hold Key #13 (or #16) and tap **Key #2** or **Key #3** to jump directly to that profile!
* **🎨 Onboard WS2812 RGB LED (GP16):**
  * **Profile 1 (Numpad):** Electric Blue (`#0082ff`)
  * **Profile 2 (Git & Dev):** Emerald Green (`#00ff3c`)
  * **Profile 3 (Snippets):** Magenta / Purple (`#dc00ff`)
  * **Profile 4 (Windows):** Gold / Amber (`#ff8c00`)
  * **Flash Save Confirmation:** Quick white pulse

---

## 🛠️ Matrix Wiring (Waveshare RP2040-Zero)

All 8 matrix wires connect down the **right side** of the RP2040-Zero:

```
                   ┌──────────────┐
                   │    USB-C     │
                   └──────────────┘
  5V             [ ]              [ ] GP0  ── Row 3 Bottom (0, ., Enter, +)
  GND            [ ]              [ ] GP1  ── Row 2 (1, 2, 3, -)
  3V3            [ ]              [ ] GP2  ── Row 1 (4, 5, 6, *)
  GP29           [ ]              [ ] GP3  ── Row 0 Top (7, 8, 9, /)
  GP28           [ ]              [ ] GP4  ── Col 0 (Left)
  GP27           [ ]              [ ] GP5  ── Col 1
  GP26           [ ]              [ ] GP6  ── Col 2
  GP15           [ ]              [ ] GP7  ── Col 3 (Right)
```
* Onboard WS2812 RGB LED is pre-wired on **GP16**.

---

## 🚀 Tagged Firmware Releases & Flashing

### 🏷️ Firmware Binary Naming Standard
Firmware binaries are tagged with the keyboard project, target MCU, board model, and release version tag so you can immediately identify the build:
* **Current Tagged Release:** [`4x4keyboard_rp2040_zero_v1.5.1.uf2`](4x4keyboard_rp2040_zero_v1.5.1.uf2)
* **Releases Archive:** [`releases/`](releases/) (contains all version-tagged UF2 builds)
* **Legacy Alias:** [`firmware.uf2`](firmware.uf2) (kept for backwards-compatible scripts and tools)

### 💡 Customizing Keys & Profiles (Zero Flashing Required!)
* You do **not** need to flash firmware to change keys, macros, scripts, hold time, or switch profiles!
* Simply open [https://saikumarmohan.github.io/saipad/](https://saikumarmohan.github.io/saipad/), click **Connect Keyboard**, customize anything, and click **"💾 Sync to Flash"**. It writes to the RP2040 internal flash in 1 millisecond.

### ⚡ Upgrading Firmware (Only when updating core code)
* **Method A (No physical buttons needed - Web Browser / 1-Click):**
  1. Open [https://saikumarmohan.github.io/saipad/](https://saikumarmohan.github.io/saipad/) and connect.
  2. Click **⚙️ Hardware** -> **⚡ Reboot to BOOTSEL**.
  3. The board reboots into bootloader mode and the **`RPI-RP2`** drive appears in Windows Explorer.
  4. Drag and drop [`4x4keyboard_rp2040_zero_v1.5.1.uf2`](4x4keyboard_rp2040_zero_v1.5.1.uf2) onto the **`RPI-RP2`** drive (or click **"🔥 1-Click Copy to RPI-RP2"** in the browser).
  5. The keyboard restarts automatically.
* **Method B (Hardware fallback):**
  1. Hold the physical **`BOOT`** button on your RP2040-Zero while plugging in the USB cable.
  2. Drag and drop [`4x4keyboard_rp2040_zero_v1.5.1.uf2`](4x4keyboard_rp2040_zero_v1.5.1.uf2) onto the **`RPI-RP2`** drive.

---

## 🤖 AI Assistant Copilot & Custom Layout Guide

You can ask any AI (**ChatGPT**, **Claude**, or **Gemini**) to design a custom 16-key profile for your favorite software, and import it directly into your keyboard with 1 click!

### Copy-Paste AI System Prompt:
```
You are a specialist mechanical keyboard macro engineer designing a custom profile for SaiPad (Waveshare RP2040-Zero).

Target Application / Workflow:
"[INSERT APPLICATION NAME HERE, e.g. Blender 3D, DaVinci Resolve, Photoshop, AutoCAD, Unreal Engine, TradingView]"

Physical Matrix Specification:
- 16 Keys in a 4x4 Matrix (Row 0: Keys #1..#4, Row 1: Keys #5..#8, Row 2: Keys #9..#12, Row 3: Keys #13..#16).
- Natural top-to-bottom layout.

Key Definition Schema:
- label: String (Max 11 chars, e.g. "git status", "Cut (C)", "Render")
- type: Integer
    0 = Single Character (code: ASCII number, e.g. 'c'=99, '7'=55)
    1 = Special Key (Enter=176, Esc=177, Bksp=178, Tab=179, Space=32, Del=212, Up=218, Down=217, Left=216, Right=215, Mute=226, Play=205, VolUp=233, VolDown=234)
    2 = Modifier Shortcut (mod bitmask: 1=Ctrl, 2=Shift, 4=Alt, 8=Win; code: ASCII key)
    3 = Text Macro (typed sequentially, e.g. "npm run dev\n")
    4 = Hardware Action (1=Next Layer, 2=Jiggler, 3=Terminal, 4=VS Code)
    5 = Script / App Launcher (Win+R command, e.g. "wt", "calc", "explorer .", "start https://...")
- mod: Integer bitmask (1=Ctrl, 2=Shift, 4=Alt, 8=Win; 0 if none)
- code: Integer keycode
- macro: String (script command if type=5, text macro if type=3, empty string otherwise)

Instructions:
1. Provide the optimal 16 keys for this application.
2. Ensure Key #16 is dedicated to layer navigation: {"label": "Next Layer", "type": 4, "code": 1, "mod": 0, "macro": ""}
3. Return ONLY a single valid JSON block formatted as:
```json
{
  "name": "Short Name",
  "category": "Creative",
  "desc": "Custom macropad profile",
  "color": "#ff7700",
  "r": 255, "g": 119, "b": 0,
  "keys": [
    { "label": "Key 1", "type": 0, "code": 99, "mod": 0, "macro": "" },
    ... exactly 16 keys
  ]
}
```
```

---

## 📄 License

The SaiPad Web Companion Studio, presets, and configuration tools are open-sourced under the [MIT License](LICENSE).
Copyright (c) 2026 Sai (Saikumar Mohan).
