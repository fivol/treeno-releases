# Treeno — Desktop Releases

This repository hosts the prebuilt **desktop binaries** for [Treeno](https://treeno.org), a tree-structured note-taking app for keyboard-first thinkers.

It is the canonical download host: it serves the in-app auto-updater and powers the download buttons on the landing page. The application source code lives elsewhere; this repo only stores the build artifacts.

## Try Treeno

- 🌐 **Landing & download page** — [treeno.org](https://treeno.org)
- 💻 **Web app** — [web.treeno.org](https://web.treeno.org) (no install needed)
- 📥 **Latest desktop release** — [Releases ↓](https://github.com/fivol/treeno-releases/releases/latest)

## What's in each release

Every release contains native installers for all desktop platforms plus the signed payloads consumed by the in-app auto-updater.

| Platform | File | Purpose |
|---|---|---|
| macOS — Apple Silicon | `Treeno_macOS_arm64.dmg` | Drag-to-Applications installer |
| macOS — Intel | `Treeno_macOS_x64.dmg` | Drag-to-Applications installer |
| Linux | `Treeno_Linux_x86_64.AppImage` | Portable binary, `chmod +x` and run |
| Linux (Debian / Ubuntu) | `Treeno_Linux_x86_64.deb` | `sudo dpkg -i` |
| Windows | `Treeno_Windows_x64-setup.exe` | NSIS installer |

The `*.app.tar.gz`, `*.AppImage.sig`, and `*-setup.exe.sig` files are auto-updater payloads — you don't need to download them manually. Same for `latest.json`, which is what the running app polls to discover new versions.

## Auto-update

Once installed, Treeno checks this repo on launch and updates itself silently in the background. Manual installs are only needed for the very first version.

## Reporting issues

Found a bug? File it at [treeno.org](https://treeno.org) or in the main project's tracker — issues filed here on `treeno-releases` will not be triaged.