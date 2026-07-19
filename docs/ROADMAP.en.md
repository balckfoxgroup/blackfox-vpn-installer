# Black Fox Vpn Installer — Roadmap

**Last updated:** 2026-07-19  
**Product:** Black Fox Vpn Installer  
**Current releases:** Windows **v1.3.0 (Build 202)** · Android **v0.4.13 (Build 21)** · Config Builder **v1.1.3 (Build 7)**  
**Website:** [https://foxnext.net](https://foxnext.net)

This roadmap describes completed work, active work, and planned work for Black Fox Group’s server-deployment suite (Windows + Android). It is based on the current Windows Go codebase, Flutter Android app, website, and licensing service behavior.

---

## Downloads (full product names)

| Product | File | Link |
|---------|------|------|
| Black Fox Vpn Installer (Windows) | `Black Fox Vpn-Installer-Setup.exe` | [Download](https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe) |
| BlackFox Vpn Android | `BlackFox-VPN-Android-release.apk` | [Download](https://foxnext.net/downloads/BlackFox-VPN-Android-release.apk) |
| Black Fox Config Builder | `Black-Fox-Config-Builder.apk` | [Download](https://foxnext.net/downloads/Black-Fox-Config-Builder.apk) |

Google Play publication for BlackFox Vpn Android: **Coming Soon**  
macOS edition: **Coming Soon**

---

## Completed

### Platform & releases

- Windows desktop installer and operations console — **Black Fox Vpn Installer** v1.3.0 Build 202  
- Android operations app — **BlackFox Vpn Android** v0.4.13 Build 21  
- Companion Android tool — **Black Fox Config Builder** v1.1.3 Build 7  
- Official site + dual update hosts (`foxnext.net`, `blackfoxupdate.ir`)  
- Privacy Policy pages (EN/FA) on foxnext.net  

### Core operations (Windows + Android)

- Basic Mode and Pro Mode  
- Central Server setup / Connect SSH / Full Deploy  
- Tunnel Server management (Pro)  
- Exit Server management (Basic: 2 slots · Pro: up to 6)  
- WireGuard primary tunnels + GRE fallback  
- Configure Panel helpers  
- Core helpers: Install WireGuard / Install 3X-UI  

### Pro advanced features

- Domain / subdomain management with DNS automation (Cloudflare, ArvanCloud)  
- CDN automation on **Windows Pro** (ArvanCloud, Cloudflare, KeyCDN, Other)  
- **Move Central Server on Windows and Android (Pro)**  
  - Reconnects tunnel and exit servers to the new central  
  - Transfers 3X-UI panel clients automatically via snapshot restore  
  - Creates a local migration backup during the move  
- Migration-oriented backup path used by Move Central  

### Licensing

- Online payment verification (TX Hash / USDT)  
- Offline activation codes  
- **License Reactivation** on Registration screen  
  - After uninstall/reinstall on the **same device**, user presses **Reactivation** / **فعال‌سازی مجدد**  
  - App restores activation from the official reactivation service using the device machine fingerprint  
  - Users no longer need to permanently keep license codes only to recover after reinstall on the same device  

### Companion — Black Fox Config Builder

- Android companion **Black Fox Config Builder** v1.1.3 Build 7  
- Download: [Black-Fox-Config-Builder.apk](https://foxnext.net/downloads/Black-Fox-Config-Builder.apk)  
- Docs repo: [balckfoxgroup/blackfox-config-builder](https://github.com/balckfoxgroup/blackfox-config-builder)  
- Six tabs: Connection · Single · Bulk · List · Settings · Contact  
- Multi-inbound create (single + bulk)  
- Delete from panel / delete from list  
- Dual-server remote updates (`blackfoxupdate.ir` + `foxnext.net`)  
- Requires 3X-UI **≥ 3.3.0** · Android API 24+ · 10 languages  
- Build 6: dual-server remote feed · Build 7: current published Android release  

### Localization

- **10 languages:** English, Persian, Russian, Chinese, German, Uzbek, Turkish, Indonesian, Ukrainian, Hindi  
- Shared localization coverage across apps and website  

### Documentation & brand surfaces

- README (EN + full FA)  
- ROADMAP (EN + FA)  
- WHITEPAPER (EN + FA)  
- Website guides for Basic / Pro / Registration / Keys / Config Builder  

---

## In Progress

- Further Android ↔ Windows operational parity (UI depth and edge-case flows)  
- UX hardening for long-running deploy / move operations  
- Stability improvements around SSH, panel sync, and update checks  
- Website content synchronization with product behavior  
- Softening remaining differences between Windows CDN tooling and Android Pro scope  

---

## Planned

### Near term

- Google Play listing for **BlackFox Vpn Android** (Coming Soon → published)  
- Broader standalone Backup / Restore tooling beyond Move Central migration backups  
- Mid-workflow resume / recovery UI for interrupted deployments  
- Expanded operator diagnostics and clearer failure recovery messages  

### Medium term

- macOS edition of Black Fox Vpn (Coming Soon)  
- Deeper multi-CDN workflow polish on Windows  
- Additional DNS / CDN provider options where demand is clear  
- Stronger audit trails for Move Central and license reactivation events  

### Longer term

- Expanded multi-region operator tooling  
- Deeper panel automation and client lifecycle helpers  
- Additional platforms / packaging channels as demand grows  

---

## Explicit non-goals (for now)

- Turning the suite into a consumer VPN client for end users  
- Claiming Google Play or macOS as already released  
- Documenting features that are not present in current Windows/Android source  

---

## Related documents

- [README.md](../README.md)  
- [WHITEPAPER.en.md](WHITEPAPER.en.md)  
- [WHITEPAPER.fa.md](WHITEPAPER.fa.md)  
- [ROADMAP.fa.md](ROADMAP.fa.md)  
- Config Builder docs: [balckfoxgroup/blackfox-config-builder](https://github.com/balckfoxgroup/blackfox-config-builder)  

---

© Black Fox Security Team
