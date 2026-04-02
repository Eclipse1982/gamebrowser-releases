# Game Browser

A real-time server browser for Quake 2 and Quake Live. Built with Tauri, React, and Rust.

## Download

**[Download Latest Release](https://github.com/Eclipse1982/gamebrowser-releases/releases/latest)**

### Windows Installers

| File | Description |
|------|-------------|
| `Game.Browser_x.x.x_x64-setup.exe` | NSIS installer (recommended) |
| `Game.Browser_x.x.x_x64_en-US.msi` | MSI installer |

## Antivirus False Positive Notice

> **Some antivirus software (including Windows Defender / SmartScreen) may flag Game Browser as suspicious.** This is a false positive.
>
> This happens because the application is not yet code-signed with an Extended Validation (EV) certificate. Unsigned or newly-signed executables are commonly flagged by heuristic-based antivirus engines — this is standard behavior for independent/open-source software and does not indicate any actual threat.
>
> **Game Browser is open-source and safe to use.** The application only connects to game master servers (Quake 2, Quake Live) and the Steam Web API to fetch server lists. It does not collect personal data, phone home, or modify system files.
>
> If you encounter a SmartScreen warning, click **"More info"** then **"Run anyway"** to proceed with installation.
>
> This binary has been submitted to Microsoft for false positive review. If your antivirus flags it, you can verify the download by checking the release checksums or building from source.

## Features

- Browse Quake 2 and Quake Live servers in real-time
- Live server pings with latency history
- Filter by map, game mode, player count, ping, and more
- Buddy list — track when friends are online and which server they're on
- Favorites — save servers you play on regularly
- Server notes — add personal notes to any server
- Player search — find players across all servers
- One-click connect to any server
- Bot filtering — bots are excluded from player counts (WallFly for Q2, ping-0 bots for QL)
- Keyboard shortcuts for fast navigation
- Light and dark themes
- Auto-updater — get new versions automatically

## Auto-Updates

The app checks for updates on launch. When a new version is available, a banner will appear with an "Update Now" button. Updates install silently in the background.

## System Requirements

- Windows 10/11 (64-bit)
- ~10 MB disk space

## Building from Source

If you prefer to build from source to avoid antivirus warnings:

```bash
git clone https://github.com/Eclipse1982/gamebrowser-tauri.git
cd gamebrowser-tauri
npm install
npx tauri build
```

The built installer will be in `src-tauri/target/release/bundle/`.

Requires: [Node.js](https://nodejs.org/) 18+, [Rust](https://rustup.rs/) 1.70+, and the [Tauri prerequisites](https://v2.tauri.app/start/prerequisites/).
