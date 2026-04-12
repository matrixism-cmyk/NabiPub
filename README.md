<div align="center">

# 🦋 NabiDrive

**원격 서버를 내 컴퓨터 드라이브처럼**
**Your remote server, as a local drive.**

[![Buy Pro](https://img.shields.io/badge/Pro-$19.99-F59E0B?style=for-the-badge)](https://nabisori.gumroad.com/l/ddpmb)
[![GitHub Release](https://img.shields.io/github/v/release/matrixism-cmyk/NabiPub?label=Download&style=for-the-badge&color=0a0)](https://github.com/matrixism-cmyk/NabiPub/releases/latest)
[![Windows](https://img.shields.io/badge/Windows_10%2F11-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/matrixism-cmyk/NabiPub/releases/latest)
[![Rust](https://img.shields.io/badge/Built_with_Rust-000000?style=for-the-badge&logo=rust&logoColor=white)](https://www.rust-lang.org/)

🇰🇷 한국어 | 🇺🇸 English — *Windows 시스템 언어에 따라 자동 전환*

</div>

---

## Why NabiDrive? | 왜 나비드라이브인가?

> **NAS나 리눅스 서버 파일을 쓸 때마다 WinSCP로 다운로드 → 수정 → 업로드하고 계신가요?**
> NabiDrive를 설치하면 원격 서버가 내 PC의 드라이브처럼 나타납니다.
> 탐색기에서 바로 열고, 수정하고, 저장하면 끝!

> **Tired of downloading, editing, and re-uploading files via WinSCP?**
> NabiDrive mounts your remote server as a local Windows drive.
> Open, edit, save — directly from Explorer!

### vs sshfs-win + sshfs-win-manager

| | NabiDrive | sshfs-win-manager | sshfs-win |
|:---|:---:|:---:|:---:|
| **GUI** | ✅ Built-in | ✅ Separate app | ❌ CLI only |
| **FTP Support** | ✅ | ❌ | ❌ |
| **Disk Cache** | ✅ 1GB LRU | ❌ | ❌ |
| **Smart Prefetch** | ✅ | ❌ | ❌ |
| **8-Channel SFTP** | ✅ | ❌ | ❌ |
| **Auto Reconnect** | ✅ 5 retries | ❌ | ❌ |
| **Auto Update** | ✅ In-app | ❌ | ❌ |
| **Custom Volume Name** | ✅ | ❌ | ❌ |
| **Multi-Language** | ✅ KR/EN | ❌ | ❌ |
| **Dark/Light Theme** | ✅ Auto | ❌ | ❌ |
| **Driver** | Dokan + ProjFS | WinFsp | WinFsp |
| **Price** | **Free** (2 drives) | Free | Free |
| **Language** | Rust | Vue/Electron | C |

### vs Commercial Products | 상용 제품과 비교

| | NabiDrive | NetDrive | Mountain Duck | SFTP Net Drive |
|:---|:---:|:---:|:---:|:---:|
| **가격 Price** | **무료 Free** | $56/yr | $39 | $40 |
| **구독 Subscription** | ❌ No | ✅ Annual | ❌ | ❌ |
| **SFTP** | ✅ | ✅ | ✅ | ✅ |
| **FTP** | ✅ | ✅ | ✅ | ❌ |
| **한국어 Korean** | ✅ | ✅ | ❌ | ❌ |
| **디스크 캐시 Cache** | ✅ | ✅ | ✅ | ❌ |
| **자동 업데이트 Update** | ✅ | ✅ | ✅ | ✅ |
| **메모리 Memory** | ~20MB | ~80MB | ~100MB | ~30MB |
| **Cloud Storage** | ❌ | ✅ | ✅ | ❌ |

> 💡 NabiDrive는 SFTP/FTP **서버 전용**입니다. Google Drive, S3 등 클라우드가 필요하면 NetDrive, Mountain Duck을 추천합니다.
> 💡 NabiDrive is for SFTP/FTP **servers only**. For cloud storage (Google Drive, S3), we recommend NetDrive or Mountain Duck.

---

## Features | 주요 기능

| Feature | 기능 | Description |
|:--------|:-----|:------------|
| 🔒 SFTP Drive | SFTP 드라이브 | SSH 기반 보안 연결, 호스트 키 자동 검증 |
| 📂 FTP Drive | FTP 드라이브 | 레거시 FTP 서버 호환 |
| 🌳 Directory Browser | 디렉토리 브라우저 | 트리뷰로 원격 폴더 탐색 후 경로 선택 |
| 💾 Disk Cache | 디스크 캐시 | 1GB LRU 캐시로 반복 접근 속도 향상 |
| ⚡ 8-Channel SFTP | 8채널 SFTP | 단일 SSH 연결에서 8개 채널 병렬 전송 |
| 🔄 Auto Reconnect | 자동 재연결 | 네트워크 끊김 시 최대 5회 자동 복구 |
| 📦 Auto Update | 자동 업데이트 | 앱 내에서 새 버전 감지 → 다운로드 → 설치 |
| 🌍 Multi-Language | 다국어 | 한국어, English (시스템 언어 자동 감지) |
| 🌗 Theme | 테마 | Windows 다크/라이트 테마 자동 감지 |
| 📌 Tray Icon | 트레이 아이콘 | 최소화 시 트레이 상주, 풍선 알림 클릭 → 드라이브 열기 |
| 🚀 Startup | 시작 프로그램 | Windows 부팅 시 자동 실행 |
| 🔐 DPAPI | 비밀번호 암호화 | Windows 자격 증명 보호로 안전 저장 |
| 🎯 Drive Mode | 드라이브 모드 | Auto / Dokan / ProjFS 프로필별 선택 |

---

## Installation | 설치

1. **[최신 인스톨러 다운로드 Download](https://github.com/matrixism-cmyk/NabiPub/releases/latest)** (`nabidrive_setup_vXXXX.exe`)
2. 인스톨러 실행 (Dokan 드라이버 자동 설치)
   Run the installer (Dokan driver installed automatically)
3. NabiDrive 실행 → 연결 추가 → 사용
   Launch NabiDrive → Add connection → Use

### System Requirements | 시스템 요구사항
- Windows 10 / 11 (64-bit)
- Internet connection

---

## Pricing | 가격

| | Free 무료 | Pro |
|:---|:---:|:---:|
| **드라이브 Drives** | 2개 | 무제한 Unlimited |
| **기능 Features** | 전체 All | 전체 All |
| **구독 Subscription** | ❌ | ❌ |

---

## Tech Stack | 기술 스택

| | |
|:---|:---|
| **Language** | Rust |
| **GUI** | egui (eframe 0.34) |
| **FS Driver** | Dokan 2.x / ProjFS fallback |
| **SSH** | russh + russh-sftp |
| **FTP** | suppaftp |
| **Installer** | NSIS (multilingual) |

---

## Nabi Promise | 나비의 약속

> *한없이 무해한 소프트웨어 — Endlessly Harmless Software*

1. ❌ 광고 없음 No ads
2. ❌ 개인정보 수집 없음 No data collection
3. ❌ 불필요한 백그라운드 통신 없음 No unnecessary network activity
4. ❌ 강제 업데이트 없음 No forced updates
5. ❌ 제거 시 흔적 없음 Clean uninstall
6. ❌ 번들 소프트웨어 없음 No bundled software

---

<div align="center">

🌐 [nabisori.kr](https://nabisori.kr) · 📥 [Download](https://github.com/matrixism-cmyk/NabiPub/releases/latest)

**Copyright © 2026 NabiSori. All rights reserved.**

</div>

---

## Open Source Licenses

### Dokan (dokany) — MIT License

```
Copyright (C) 2015-2020 Adrien J., Maxime C.
Copyright (C) 2007-2011 Hiroki Asakawa

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software...
```

Full license: [THIRD_PARTY_LICENSES.txt](https://github.com/dokan-dev/dokany/blob/master/license.mit.txt)
