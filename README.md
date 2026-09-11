# CyberAudio Patchbox OS for Raspberry Pi 5 (Debian Bookworm ARM64)

[![Release](https://img.shields.io/github/v/release/danny1marshall1587-maker/CyberAudio-PatchboxOS-Pi5-AutoMODEP?color=00ff66&label=Release)](https://github.com/danny1marshall1587-maker/CyberAudio-PatchboxOS-Pi5-AutoMODEP/releases/latest)
[![Architecture](https://img.shields.io/badge/Architecture-ARM64%20(aarch64)-blue)](#)
[![OS](https://img.shields.io/badge/OS-Debian%2012%20(Bookworm)-red)](#)
[![Target](https://img.shields.io/badge/Platform-Raspberry%20Pi%205-purple)](#)

A ready-to-flash, pre-configured **Patchbox OS (Debian 12 Bookworm ARM64)** image tailored specifically for guitarists, producers, and live performers using the **Raspberry Pi 5**.

---

## Key Pre-Configured Features

### 1. Zero-Login Auto-Run MODEP
- Boots straight into MODEP without needing a keyboard, monitor, or user login.
- `modep-mod-ui` and `modep-mod-host` launch automatically as systemd background services on port 80.
- `tty1` console autologin is pre-configured for the `patch` user without password prompts.

### 2. Dual-Mode Intelligent Networking
- **Home Wi-Fi Auto-Connect**:
  - Automatically joins your home Wi-Fi (`VM99103602.4g`) with highest autoconnect priority (`100`).
  - Access MODEP directly at `http://patchbox.local` or your Pi's local network IP.
- **Fallback Hotspot**:
  - Automatically broadcasts an access point named **`patchbox`** (Password: **`blokaslabs`**) when away from home or when home Wi-Fi is disconnected.
  - Connect your smartphone, tablet, or laptop directly to the hotspot and open `http://172.24.1.1` or `http://patchbox.local`.

### 3. Complete Cyber Audio Master Suite (94 Pre-Loaded LV2 Plugins)
- **Evans Bass Tribute Pedal**: Intelligent auto-bass player with Parkinson's tribute dedication, walking groove algorithms, and strict logic controls.
- **4 Boutique Studio Delays**: Cyber PureSustain Delay, Horizon Tape Echo, CyberShimmer Ambient Delay, and Crystal Echo Modulated Delay.
- **3 Algorithmic Reverbs**: CyberVerb Pro, Shimmer Hall, and Bloom Reverb.
- **20 Re-Voiced Cyber Amps**: Featuring high-gain, edge-of-breakup, acoustic, and clean boutique amp captures.
- **Full Pedalboard Suite**: Complete collection of drives, distortions, modulation, and filters with customized native MOD-GUIs.

### 4. Integrated Cyber Strobe & Peak Tuner
- Directly embedded into the MODEP top navigation bar.
- Ultra-precise pitch tracking, Peterson sweetened tunings, and James Taylor acoustic offsets.
- Full MIDI assignment support with persistent recall across pedalboard changes.

---

## Direct Download & Flashing

### 1. Download
Get the pre-configured image archive from the latest release:
- **[Download CyberAudio-PatchboxOS-Pi5-AutoMODEP.7z (1.50 GB)](https://github.com/danny1marshall1587-maker/CyberAudio-PatchboxOS-Pi5-AutoMODEP/releases/download/v1.0.0/CyberAudio-PatchboxOS-Pi5-AutoMODEP.7z)**

### 2. Flash to MicroSD Card
1. Extract `CyberAudio-PatchboxOS-Pi5-AutoMODEP.7z` using [7-Zip](https://www.7-zip.org/) to obtain `2024-04-04-Patchbox.img`.
2. Open **[Raspberry Pi Imager](https://www.raspberrypi.com/software/)** or **[Rufus](https://rufus.ie/)**.
3. Choose **Use Custom Image** and select `2024-04-04-Patchbox.img`.
4. Choose your MicroSD card (32 GB or larger recommended) and click **Write**.

### 3. Boot Your Raspberry Pi 5
1. Insert the card into your Raspberry Pi 5 and connect power.
2. The system self-initializes all 94 plugins, network profiles, and autologin on first boot.
3. Open `http://patchbox.local` (or `http://172.24.1.1` on the `patchbox` hotspot) in any web browser and play!
