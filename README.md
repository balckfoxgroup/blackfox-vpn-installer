<p align="center">
  <img src="docs/assets/logo.jpg" alt="Black Fox VPN Logo" width="96">
</p>

<h1 align="center">Black Fox Vpn Installer</h1>

<p align="center">
  <strong>Server Deployment Automation · Multi-Location VPN Infrastructure</strong><br>
  Windows &amp; Android · WireGuard + 3X-UI (Sanaei)
</p>

<p align="center">
  <a href="https://foxnext.net">Website</a> •
  <a href="https://foxnext.net/en/privacy.html">Privacy</a> •
  <a href="https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe">Windows</a> •
  <a href="https://foxnext.net/downloads/BlackFox-VPN-Android-release.apk">Android</a> •
  <a href="https://github.com/balckfoxgroup/blackfox-config-builder">Config Builder</a> •
  <a href="https://t.me/blackFoxVPNN">Telegram</a> •
  <a href="https://github.com/balckfoxgroup/blackfox-vpn-installer">GitHub</a>
</p>

---

## 1. Project Introduction

**Black Fox Vpn Installer** is **not** a simple VPN client.

It is a suite of **server management and deployment tools** for:

- Server Deployment Automation  
- Multi-Server Infrastructure Management  
- VPN Infrastructure Configuration  
- Central Server Management  
- Tunnel Management  
- Exit Server Management  
- Backup and Restore during Central Server migration  

The software is designed for environments with restricted global connectivity and helps operators deploy multi-location VPN infrastructure **without deep Linux expertise**.

### What's available now

| Platform | Product | Status |
|----------|---------|--------|
| Windows | Black Fox Vpn Installer | **Available** — v1.3.0 (Build 202) |
| Android | BlackFox Vpn Android | **Available** — v0.4.13 (Build 21) |
| Android | Black Fox Config Builder | **Available** — v1.1.3 (Build 7) |
| Android | Google Play | **Coming Soon** |
| macOS | Black Fox Vpn | **Coming Soon** |

> The Android edition of BlackFox is released and can be downloaded from the official Black Fox Group website. Google Play publication is Coming Soon.

---

## 2. Features

- Automated 3X-UI (Sanaei) installation and panel configuration  
- WireGuard primary tunnels + GRE fallback  
- Basic Mode and Pro Mode workflows  
- Central / Tunnel / Exit server operations  
- Domain & subdomain management (Pro)  
- CDN automation on Windows Pro  
- Move Central Server with automated panel client transfer  
- Dual update hosts (`foxnext.net` + `blackfoxupdate.ir`)  
- Official website and Privacy Policy pages  

<p align="center">
  <img src="docs/assets/page-0.png" alt="Basic Mode vs Pro Mode" width="520">
</p>

---

## 3. Basic Mode

Basic Mode is for operators who need a **simpler and faster** structure:

- Central Server Setup  
- Connect SSH / Full Deploy  
- Exit servers (slots 1–2)  
- Configure Panel  
- Core helpers (Install WireGuard / Install 3X-UI)  

<p align="center">
  <img src="docs/assets/dashboard-basic.png" alt="Basic Mode dashboard" width="520">
</p>

---

## 4. Pro Mode

Pro Mode is for **advanced multi-server infrastructure**:

- Central Server  
- Tunnel Server  
- Exit Server (up to 6)  
- WireGuard + GRE  
- Domain / DNS management  
- CDN providers (Windows)  
- Move Central Server  
- Migration backup + automated client continuity  

<p align="center">
  <img src="docs/assets/dashboard-pro.png" alt="Pro Mode dashboard" width="520">
</p>

---

## 5. Android Version

**BlackFox Vpn Android is released.**

- Download: [BlackFox-VPN-Android-release.apk](https://foxnext.net/downloads/BlackFox-VPN-Android-release.apk)  
- Current version: **0.4.13 (Build 21)**  
- Google Play: **Coming Soon**  

Users can download the official Android build from the Black Fox Group website today. A Google Play listing is planned and will be announced when available.

<p align="center">
  <img src="docs/assets/android-dashboard.png" alt="BlackFox Vpn Android" width="48%">
  &nbsp;
  <img src="docs/assets/android-vpn/choose-mode-duo.png" alt="Choose Mode" width="48%">
</p>

<p align="center">
  <img src="docs/assets/android-vpn/basic-mode-duo.png" alt="Android Basic" width="32%">
  <img src="docs/assets/android-vpn/pro-mode-duo.png" alt="Android Pro" width="32%">
  <img src="docs/assets/android-config-builder.png" alt="Config Builder" width="32%">
</p>

<p align="center"><em>Android VPN · Config Builder</em></p>

More Android notes: [Mobile/README.md](Mobile/README.md)

---

## 6. Windows Version

- Product: **Black Fox Vpn Installer**  
- Version: **1.3.0 (Build 202)**  
- Download: [Black Fox Vpn-Installer-Setup.exe](https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe)  

Windows remains the full desktop operations console for Basic and Pro infrastructure workflows.

---

## 7. Supported Languages

BlackFox Group applications are designed for a global audience and support **10 major living languages**:

1. English  
2. Persian (Farsi)  
3. Russian  
4. Chinese  
5. German  
6. Uzbek  
7. Turkish  
8. Indonesian  
9. Ukrainian  
10. Hindi  

Coverage includes current app editions and the website at [foxnext.net](https://foxnext.net).

---

## 8. Architecture

```text
Central Server
      ↓
Tunnel Server
      ↓
Exit Server
      ↓
Client Infrastructure
```

The application simplifies installation, configuration, and day-to-day management of this chain.

---

## 9. WireGuard and GRE

- **WireGuard** is the primary tunnel technology  
- **GRE** is available as a fallback path when WireGuard cannot sustain the route  
- Exit servers provide egress; tunnel servers act as relays in Pro Mode  

---

## 10. Central / Tunnel / Exit Servers

| Role | Purpose |
|------|---------|
| Central Server | Hub with 3X-UI panel and orchestration point |
| Tunnel Server | Optional Pro multi-hop relay |
| Exit Server | Internet egress location |

Basic Mode focuses on Central + limited Exit slots. Pro Mode adds Tunnel servers and expanded Exit capacity.

---

## 11. Domain Management

In Pro Mode, operators can manage domains/subdomains with DNS automation.

Current DNS providers in product flows include:

- Cloudflare  
- ArvanCloud  

Windows Pro also includes CDN operations for:

- ArvanCloud  
- Cloudflare  
- KeyCDN  
- Other CDN  

---

## 12. Privacy Policy

A dedicated Privacy Policy is published on the official website.

Users can review data-handling statements here:

- English: [https://foxnext.net/en/privacy.html](https://foxnext.net/en/privacy.html)  
- Persian: [https://foxnext.net/fa/privacy.html](https://foxnext.net/fa/privacy.html)  

Please treat those pages as the authoritative privacy source for Black Fox Group Installer products.

---

## 13. Roadmap

See the living roadmap documents:

- English: [docs/ROADMAP.en.md](docs/ROADMAP.en.md)  
- Persian: [docs/ROADMAP.fa.md](docs/ROADMAP.fa.md)  

Whitepaper:

- English: [docs/WHITEPAPER.en.md](docs/WHITEPAPER.en.md)  
- Persian: [docs/WHITEPAPER.fa.md](docs/WHITEPAPER.fa.md)  

Highlights:

| Status | Examples |
|--------|----------|
| Completed | Windows + Android releases, 10 languages, Basic/Pro, Move Central, WireGuard/GRE, Domain/CDN |
| In Progress | UX hardening, Android/Windows parity improvements |
| Planned | macOS, Google Play listing, broader Backup/Restore, mid-workflow resume UI |

---

## 14. Support the Project

If BlackFox VPN Installer is useful to you, please support Black Fox Group development by giving the repository a star.

- Star the Repository  
- Report Bugs  
- Suggest Features  
- Share the Project  
- Support the Development  

Channels:

- Telegram: [https://t.me/blackFoxVPNN](https://t.me/blackFoxVPNN)  
- Website: [https://foxnext.net](https://foxnext.net)  
- GitHub: [https://github.com/balckfoxgroup](https://github.com/balckfoxgroup)  
- Email: support@foxnext.net  

---

## 15. License

Commercial product. Licensing tiers (Basic / Pro) are managed through the official registration flows on [foxnext.net](https://foxnext.net).

---

## فارسی (خلاصه)

Black Fox مجموعه ابزارهای **مدیریت و راه‌اندازی سرور** است، نه یک کلاینت VPN ساده. نسخه ویندوز و نسخه اندروید منتشر شده‌اند. Google Play برای اندروید **به‌زودی** است. macOS نیز در برنامه است.

| منبع | لینک |
|------|------|
| وب‌سایت | [foxnext.net](https://foxnext.net) |
| حریم خصوصی | [foxnext.net/fa/privacy.html](https://foxnext.net/fa/privacy.html) |
| ویندوز | [Setup.exe](https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe) |
| اندروید | [APK](https://foxnext.net/downloads/BlackFox-VPN-Android-release.apk) |
| نقشه راه | [docs/ROADMAP.fa.md](docs/ROADMAP.fa.md) |
| وایت‌پیپر | [docs/WHITEPAPER.fa.md](docs/WHITEPAPER.fa.md) |

**۱۰ زبان:** انگلیسی، فارسی، روسی، چینی، آلمانی، ازبکی، ترکی، اندونزیایی، اوکراینی، هندی.

اگر این پروژه برای شما مفید است، با Star کردن Repository از توسعه Black Fox Group حمایت کنید.

---

© Black Fox Security Team
