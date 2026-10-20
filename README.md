
[![GitHub Release](https://img.shields.io/github/v/release/LibbyLamarr/Uniden-Desktop-Control?color=orange&label=release)](https://github.com/LibbyLamarr/Uniden-Desktop-Control/releases/latest)
![Platforms](https://img.shields.io/badge/platforms-Windows%20%7C%20Android-blue)
![Status](https://img.shields.io/badge/status-In%20Development-yellow)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-Support%20UDC-FFDD00?logo=buymeacoffee&logoColor=black)](https://buymeacoffee.com/libbylamarr)


# 📡 Uniden Desktop Control (UDC)

**A virtual scanner console, channel memory manager and audio logging companion for Uniden BC125-series scanners.**

Uniden Desktop Control (UDC) is a hobby project designed to make controlling and programming a scanner from a computer easier — with a compact, realistic-looking console for everyday use and a full view for more advanced tasks.

UDC supports the **Uniden Bearcat BC125AT** (US/Canada/Australia) and **UBC125XLT / UBC125XLTC** (UK/Europe) analogue radio scanners. It is available as a Windows desktop application and has also been ported to Android with USB-OTG support.

> **Development status:** UDC is still a work in progress. Some features may contain bugs or behave unexpectedly. **Back up your scanner's channel configuration before making changes.** Feedback and bug reports are welcome!

## 🖼️ Screenshots

### Compact console — the default view

The compact console was the original reason I started this project: a small, convenient way to control my scanner from a PC without taking up much screen space.

<p align="center">
  <img src="screenshots/compact%20view.png" alt="UDC default compact scanner console" width="360">
</p>

### Full view

Switch to the full interface when you need channel management and the additional tools.

![UDC full application view](screenshots/full%20view.png)

<details>
<summary><strong>More screenshots — menu navigation, recent hits and audio recording</strong></summary>

#### Menu navigation

![UDC menu navigation](screenshots/menu%20navigation.png)

#### Recent hits

![UDC recent hits dashboard](screenshots/recent%20hits.png)

#### Audio recording

![UDC audio recording interface](screenshots/audio%20recording.png)

</details>

## 📥 Downloads

Check the [Releases page](https://github.com/LibbyLamarr/Uniden-Desktop-Control/releases) for downloadable builds **when available**.

- **Windows:** UDC is designed to run as a self-contained x64 desktop executable (`UDC.exe`).
- **Android:** An Android version (`.apk`) supports USB-OTG connections to compatible scanners.

> Release files and installation instructions will be updated as builds become available. Android USB support requires compatible hardware and an appropriate USB-OTG cable or adapter.

## 📻 Supported scanners

- **BC125AT** — US, Canada and Australia
- **UBC125XLT / UBC125XLTC** — UK and Europe

UDC communicates using Uniden's remote control protocol, including `KEY`, `GLG`, `STS` and `CIN` commands.

Note: Confirmed working with UBC125XLTC scanner only.

## ✨ Features

### 📺 Live display and virtual console

- Real-time LCD mirroring based on `STS` and `GLG` telemetry polling.
- Interactive four-row menu navigator for browsing scanner menus.
- Choice of LCD backlight colours: Uniden Amber, Marine Teal, Ice Blue, Emerald Green, Sunset Orange and Ruby Red.
- Channel tags, aviation frequency display (8.33 kHz and 12.5 kHz) and a live signal meter.
- Compact and full-size layouts for different ways of using the application.

### 🗂️ 500-channel bank memory manager

- Read and write all 10 banks, with 50 channels per bank.
- Edit frequencies, modulation, CTCSS/DCS tones, delay, lockout and priority.
- Toggle scan banks using on-screen chassis buttons and LED indicators.
- Tune directly to a hardware channel using the `HOLD` → `CH` → `HOLD` sequence.

### 🔄 Import and export

- Standard CSV formats used by Bearpaw and bc125py.
- Native Uniden software format (`.bc125at_ss`).
- Scan125 / Scan125 Convert format (`.c125`).
- `CIN` command script export.
- Import or export individual banks or all banks, with previews and target-bank mapping.

### 🎙️ Audio recording and transmission logging

- Record scanner audio from its 3.5 mm headphone/line-out connection to a suitable audio input.
- Voice-activated / squelch-triggered recording and MP3 encoding using `lame.js`.
- Audio VU meter, transmission duration tracking, in-app playback and batch recording management.

### 📊 Recent hits

- Track recent transmissions with frequency, channel name, hit count, signal strength and timestamps.
- Select a recent hit to tune back to that frequency.

### 💻 Platforms

- **Windows:** Self-contained x64 executable with compact and full-view modes.
- **Android:** USB-OTG serial communication (`CdcAcmSerialDriver`), landscape-optimised responsive layout and automatic scaling for phones and tablets.

## 🔌 Getting started

1. Connect a supported scanner to your Windows PC or compatible Android device using an appropriate USB cable.
2. Start the corresponding UDC application build.
3. Use the app's scanner connection controls to establish communication.
4. Start with the compact console, or switch to the full view for channel management and other tools.
5. **Before writing channel data to the scanner, back up your existing programming.**

Exact connection and installation steps may vary by platform and will be expanded as releases are published.

## 🛠️ Development status and feedback

UDC is a personal project, shared in case other scanner enthusiasts find it useful. It has been developed with AI assistance against Uniden's documented remote control protocol, and I am continuing to test, fix and improve its features.

If you encounter a problem or have a suggestion, please [open a GitHub Issue](https://github.com/LibbyLamarr/Uniden-Desktop-Control/issues). When reporting a bug, it helps to include your scanner model, Windows/Android version, what you were doing and what happened.

**Use at your own risk.** This project is provided without warranty, and it is not affiliated with or endorsed by Uniden.

## ❤️ Why I made this

I originally wanted a compact, attractive front end to control my scanner from my PC. That became UDC's default compact view. The full view grew from there, adding channel programming and more advanced features.

I later ported the application to Android so I could update channels while on the go. The mobile interface is not quite as comfortable as the desktop version, but it is functional, and I plan to keep improving it.

I'm new to releasing software, and UDC began as something for my own use. I'm happy to share it with others and welcome feedback.

## 🙏 Inspiration and acknowledgements

This project was inspired in part by other useful scanner software, especially:

- [Scan125](https://www.nick-bailey.co.uk/scan125/)
- [Bearpaw](https://github.com/jeremyfuksa/bearpaw)

## 📄 Licence

No licence is specified here yet. If source code is published, please check the repository for a `LICENSE` file before assuming it may be reused or redistributed.


---

## ☕ Support the Project

Uniden Desktop Control started as a personal hobby project, created to make controlling and programming my Uniden scanner a little easier.

I've made it freely available in the hope that others might find it useful too.

If you enjoy using UDC and would like to support its continued development, you're very welcome to buy me a coffee! It's entirely optional, but always appreciated.

<a href="https://buymeacoffee.com/libbylamarr">
  <img
    src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png"
    alt="Buy Me a Coffee"
    width="180">
</a>

Thank you for trying UDC, and happy scanning! 📡
