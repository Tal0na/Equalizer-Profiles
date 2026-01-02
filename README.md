# Equalizer Profiles

[![en](https://img.shields.io/badge/lang-en-red.svg)](README.md)
[![pt-BR](https://img.shields.io/badge/lang-pt--BR-green.svg)](README.pt-BR.md)
[![ru](https://img.shields.io/badge/lang-ru-yellow.svg)](README.ru.md)
[![uk-UA](https://img.shields.io/badge/lang-uk--UA-blue)](README.uk-UA.md)

## Introduction

This repository contains **custom equalizer profiles** designed to improve audio quality on both **Windows and Linux** systems.  
The profiles focus on music listening and general multimedia use and can be adjusted according to personal taste and audio hardware.

---

## Supported Platforms & Applications

### Windows
- **Equalizer APO**
- **Peace Equalizer** (GUI for Equalizer APO)

### Linux
- **EasyEffects** (PipeWire – recommended)
- **PulseEffects** (PulseAudio – legacy)
- **PipeWire native equalizer filters**

> ⚠️ Most modern Linux distributions (Fedora, Arch, Ubuntu 22.10+) use **PipeWire** by default.  
> In this case, **EasyEffects** is the recommended application.

---

## Requirements

### Windows
- **Equalizer APO**  
  https://sourceforge.net/projects/equalizerapo/
- **Peace Equalizer**  
  https://sourceforge.net/projects/peace-equalizer-apo-extension/

### Linux
- **EasyEffects**
  - Flatpak (recommended):
    ```bash
    flatpak install flathub com.github.wwmm.easyeffects
    ```
  - Or install via your distribution’s package manager
- **PipeWire** (usually installed by default)

---

## How to Apply Profiles

### Windows (Peace Equalizer)

1. Open **Peace Equalizer**.
2. Configure the frequency bands and filters according to the profile.
3. Click **Save settings** and name your profile  
   Example: `MyEQConfig`.
4. To load a profile:
   - Open Peace Equalizer
   - Go to **Presets**
   - Select `MyEQConfig`

---

### Linux (EasyEffects)

1. Open **EasyEffects**.
2. Enable the **Equalizer** effect.
3. Configure the frequency bands manually or import a preset.
4. Click **Presets → Save Preset**.
5. (Optional) Assign the preset to:
   - System output
   - Specific applications

> EasyEffects supports **per-application profiles**, which is not available in Equalizer APO.

---

## Profile Compatibility Notes

- Frequency bands and gain values are **fully transferable** between:
  - Peace Equalizer ↔ EasyEffects
- Some filter names may differ:
  - **Preamp** → **Input Gain**
  - **Peak Filter** → **Bell Filter**
- Always adjust **preamp/input gain** to prevent audio clipping.

---

## Final Considerations

These equalizer profiles are based on **personal preferences** and may not suit all:
- Headphones or speakers
- Music genres or listening styles

Feel free to tweak:
- Gain levels
- Q values
- Preamp volume

If you improve or adapt a profile for a specific device, consider sharing it with the community.

---

## References

- Equalizer APO Documentation  
  https://sourceforge.net/p/equalizerapo/wiki/Documentation/
- Peace Equalizer User Guide  
  https://sourceforge.net/p/peace-equalizer-apo-extension/wiki/Documentation/
- EasyEffects Documentation  
  https://github.com/wwmm/easyeffects
