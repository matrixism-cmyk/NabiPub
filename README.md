# 나비 (Nabi) — 한없이 무해한 소프트웨어

나비 제품군의 공식 배포 저장소입니다.

> 광고 없음 · 개인정보 수집 없음 · 강제 업데이트 없음 · 완전 무료

---

## 제품 목록

### 나비 드라이브 (NabiDrive)

Windows용 SFTP/FTP 가상 드라이브. 원격 서버를 로컬 드라이브처럼 사용합니다.

- Dokan 가상 드라이브 마운트
- SFTP / FTP 보안 연결
- 디스크 LRU 캐시, 스마트 프리페치
- Windows 탐색기 완벽 통합

**[다운로드](https://github.com/matrixism-cmyk/NabiPub/releases)**

---

### 나비 로드셀 모니터 (Nabi LoadCell Monitor)

전자저울의 측정값을 실시간으로 PC + 태블릿에서 모니터링하는 프로그램입니다.

- RS232 시리얼 저울 연결 (CH340 USB-Serial)
- 실시간 GUI 그래프 (60fps)
- MQTT로 서버 전송 → 태블릿 브라우저에서 실시간 확인
- 저울 4모드 지원 (Auto/Hand/Contin/Ctrl)
- 시스템 트레이 상주, 자동 연결

**[다운로드](https://github.com/matrixism-cmyk/NabiPub/releases)**

---

## 시스템 요구사항

- Windows 10/11 (64비트)

### 나비 드라이브 추가 요구사항
- Dokan 드라이버 (인스톨러에서 자동 설치)

### 나비 로드셀 모니터 추가 요구사항
- USB-RS232 어댑터 (CH340)
- MQTT 브로커 (태블릿 모니터링 시)

---

## 설치

[Releases](https://github.com/matrixism-cmyk/NabiPub/releases) 페이지에서 최신 버전을 다운로드하세요.

| 파일 | 제품 |
|------|------|
| `NabiDrive_Setup_vX.X.X.exe` | 나비 드라이브 인스톨러 |
| `NabiLoadCell_vX.X.X.exe` | 나비 로드셀 모니터 (단일 실행 파일) |

---

## 웹사이트

[https://nabisori.kr](https://nabisori.kr)

---

Copyright (C) 2026 NabiSori. All rights reserved.
