# NabiDrive

**Your remote server, as a local drive.**

Mount SFTP/FTP servers as Windows drives. Copy, edit, delete files — as naturally as on your own PC.

[![GitHub Release](https://img.shields.io/github/v/release/matrixism-cmyk/NabiPub?label=Download&color=0a0)](https://github.com/matrixism-cmyk/NabiPub/releases/latest)

> 🇰🇷 한국어 | 🇺🇸 English — Auto-detected based on your Windows language

---

## Features

| Feature | Description |
|---------|-------------|
| **SFTP/FTP Drive Mount** | SSH-based secure connection with host key verification |
| **Dokan + ProjFS** | Dokan virtual drive (priority) with ProjFS fallback |
| **Directory Browser** | Tree view to browse and select remote paths |
| **Disk Cache (1GB LRU)** | Cached files for faster repeated access |
| **Smart Prefetch** | Predicts and pre-downloads frequently used files |
| **SFTP 8-Channel Pool** | Parallel transfers for better performance |
| **Auto Reconnect** | Up to 5 retries with exponential backoff |
| **Auto Update** | In-app update check, download, and install |
| **Multi-Language** | Korean, English (extensible) |
| **Dark/Light Theme** | Follows Windows system theme |
| **Tray Icon** | Minimizes to tray, balloon notifications |
| **Startup Launch** | Optional Windows startup registration |
| **DPAPI Encryption** | Passwords stored securely via Windows DPAPI |

## Screenshots

> Coming soon — clean screenshots will be added

<!-- 
![Main Screen](screenshots/main.png)
![Connection Form](screenshots/form.png)
![Directory Browser](screenshots/browser.png)
-->

## Installation

1. Download **[nabidrive_setup_vXXXX.exe](https://github.com/matrixism-cmyk/NabiPub/releases/latest)** from Releases
2. Run the installer (Dokan driver is installed automatically)
3. Launch NabiDrive and add your first connection

### System Requirements
- Windows 10/11 (64-bit)
- Internet connection

## Comparison

| | NabiDrive | NetDrive | SFTP Net Drive | Mountain Duck | Rclone |
|---|:---:|:---:|:---:|:---:|:---:|
| **Price** | **Free** (2) | $56/yr | $40 | $39 | Free |
| **SFTP** | ✅ | ✅ | ✅ | ✅ | ✅ |
| **FTP** | ✅ | ✅ | ❌ | ✅ | ✅ |
| **GUI** | ✅ | ✅ | ✅ | ✅ | ❌ (CLI) |
| **Korean** | ✅ | ✅ | ❌ | ❌ | ❌ |
| **Disk Cache** | ✅ | ✅ | ❌ | ✅ | ✅ |
| **Auto Update** | ✅ | ✅ | ✅ | ✅ | ❌ |
| **Subscription** | **No** | Annual | No | No | No |

## Pricing

- **Free**: Up to 2 drive connections
- **Pro License**: Unlimited drives, priority support

## Tech Stack

- **Language**: Rust
- **GUI**: egui (eframe 0.34)
- **FS Driver**: Dokan 2.x / ProjFS
- **SSH**: russh + russh-sftp
- **FTP**: suppaftp

## Links

- 🌐 Website: [https://nabisori.kr](https://nabisori.kr)
- 📥 Download: [Latest Release](https://github.com/matrixism-cmyk/NabiPub/releases/latest)

---

**Copyright © 2026 NabiSori. All rights reserved.**
