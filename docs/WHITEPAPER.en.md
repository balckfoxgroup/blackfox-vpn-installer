# Black Fox Vpn Installer — Whitepaper

**Last updated:** 2026-07-19  
**Product family:** Black Fox Vpn Installer (Windows) · BlackFox Vpn Android · Black Fox Config Builder  
**Current releases:** Windows **v1.3.0 (Build 202)** · Android **v0.4.13 (Build 21)** · Config Builder **v1.1.3 (Build 7)**  
**Website:** [https://foxnext.net](https://foxnext.net)  
**GitHub:** [https://github.com/balckfoxgroup/blackfox-vpn-installer](https://github.com/balckfoxgroup/blackfox-vpn-installer)

---

## 1. Purpose

Black Fox Vpn Installer is a **server deployment and operations suite**, not a consumer VPN client.

It exists to help operators in constrained networks deploy and manage multi-location VPN infrastructure built on:

- **3X-UI (Sanaei)** as the panel layer  
- **WireGuard** as the primary tunnel  
- **GRE** as a fallback path when WireGuard cannot sustain the route  

The product goal is to remove most of the repetitive Linux, SSH, panel, DNS, and tunnel work from day-to-day operations.

---

## 2. Product surfaces

| Surface | Full product name | Role | Download |
|---------|-------------------|------|----------|
| Windows | **Black Fox Vpn Installer** | Full desktop operations console | [Black Fox Vpn-Installer-Setup.exe](https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe) |
| Android | **BlackFox Vpn Android** | Mobile operations app (Basic + Pro) | [BlackFox-VPN-Android-release.apk](https://foxnext.net/downloads/BlackFox-VPN-Android-release.apk) |
| Android companion | **Black Fox Config Builder** | Config construction helper | [Black-Fox-Config-Builder.apk](https://foxnext.net/downloads/Black-Fox-Config-Builder.apk) |
| Google Play | BlackFox Vpn Android listing | Distribution channel | **Coming Soon** |
| macOS | Black Fox Vpn | Future desktop edition | **Coming Soon** |

---

## 3. Operating model

### Basic Mode

Basic Mode targets faster, smaller deployments:

- Central Server setup  
- SSH connect and Full Deploy  
- Up to two Exit servers  
- Panel configuration helpers  
- Core install helpers for WireGuard and 3X-UI  

### Pro Mode

Pro Mode targets larger multi-hop infrastructures:

- Central Server  
- Tunnel Server  
- Up to six Exit servers  
- WireGuard + GRE  
- Domain / DNS management  
- CDN automation on Windows  
- **Move Central Server on Windows and Android**  
- Migration backup during central relocation  

```text
Central Server
      ↓
Tunnel Server
      ↓
Exit Server
      ↓
Client Infrastructure
```

---

## 4. Move Central Server

Relocating the central role used to mean rebuilding tunnels, re-binding exits, and manually restoring panel clients.

**Move Central Server** automates that relocation in Pro Mode on **both Windows and Android**.

Operator flow:

1. Open Operations in Pro Mode  
2. Choose Move Central Server  
3. Enter the new central server details  
4. Let the suite reconnect tunnel and exit roles to the new central  
5. Allow automated transfer of 3X-UI panel clients from the migration snapshot  
6. Keep the local migration backup created during the move  

This is an active Android feature as well as a Windows feature. Documentation that lists Move Central as Windows-only is outdated.

---

## 5. Licensing and Reactivation

Licensing supports three practical paths:

1. Online verification through payment / TX Hash  
2. Offline activation codes  
3. **Reactivation** after reinstall on the same device  

### Why Reactivation exists

Operators often uninstall and reinstall the app. Requiring permanent storage of offline codes for that common case creates friction and support load.

### Current reactivation behavior

On the Registration screen:

1. Reinstall the app on the **same device**  
2. Open Registration  
3. Press **Reactivation** (English) / **فعال‌سازی مجدد** (Persian)  

The app uses the device’s machine fingerprint to query the official reactivation service. If a valid prior activation record exists for that device, access is restored without forcing the user to keep and re-enter a stored license code for that recovery path.

Important clarifications:

- Reactivation is for previously activated devices recorded by the official service  
- Online TX and offline codes remain available  
- Local Windows vault restore (if present) is a separate local-device mechanism and must not be confused with server reactivation  
- Reactivation does not invent a new license; it restores a known device-bound activation record  

Current public website pricing reference: Basic **19 USDT** · Pro **33 USDT** (confirm on site).

---

## 6. Domains, DNS, and CDN

Pro Mode includes domain/subdomain management with DNS automation for:

- Cloudflare  
- ArvanCloud  

Windows Pro additionally exposes CDN operations for:

- ArvanCloud  
- Cloudflare  
- KeyCDN  
- Other CDN  

Android Pro currently focuses on core topology operations and Move Central; Windows remains the deeper CDN automation surface.

---

## 7. Localization

BlackFox Group applications and the website support **10 languages**:

English, Persian, Russian, Chinese, German, Uzbek, Turkish, Indonesian, Ukrainian, Hindi.

---

## 8. Privacy and updates

- Privacy Policy EN: [https://foxnext.net/en/privacy.html](https://foxnext.net/en/privacy.html)  
- Privacy Policy FA: [https://foxnext.net/fa/privacy.html](https://foxnext.net/fa/privacy.html)  
- Update hosts: `foxnext.net` and `blackfoxupdate.ir`  

Treat the published Privacy Policy pages as the authoritative source.

---

## 9. What this suite is not

- Not a simple end-user VPN client  
- Not a claim that Google Play is already live  
- Not a claim that macOS is already shipping  
- Not a documentation surface for unimplemented features  

---

## 10. Related documents

- [README.md](../README.md)  
- [ROADMAP.en.md](ROADMAP.en.md)  
- [ROADMAP.fa.md](ROADMAP.fa.md)  
- [WHITEPAPER.fa.md](WHITEPAPER.fa.md)  
- [Mobile/README.md](../Mobile/README.md)  

---

© Black Fox Security Team
