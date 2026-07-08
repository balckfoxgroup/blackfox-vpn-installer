<p align="left">
  <img src="assets/logo.jpg" alt="Black Fox VPN" width="120" align="right">
</p>

# Whitepaper — Black Fox Vpn Installer

**Version:** 1.3.0 | **Build:** 194

[نسخه فارسی](WHITEPAPER.fa.md)

---

## 1. Executive Summary

**Black Fox Vpn Installer** is a commercial Windows desktop application that automatically deploys multi-location VPN infrastructure by connecting to Linux servers over SSH.

Users without deep Linux knowledge can:

- Deploy a central server with the 3X-UI panel
- Add exit servers in multiple countries
- Build relay tunnel chains in Pro Mode
- Configure CDN and DNS

---

## 2. Problem Statement

Deploying multi-location VPN infrastructure typically requires:

- Manual WireGuard installation
- 3X-UI panel configuration
- SSH and firewall management
- Connecting foreign servers to a central hub

This process is time-consuming and error-prone for non-technical users.

---

## 3. Solution

The application unifies all steps in a single graphical dashboard:

```
Initial Server Setup → Connect SSH → Full Deploy → Exit Servers → Configure Panel
```

<p align="center">
  <img src="assets/page-0.png" alt="Basic and Pro architecture" width="650">
</p>

---

## 4. Network Architecture

### 4.1 — Basic Mode

```
[Windows Client] → SSH → [Central Server: WireGuard + 3X-UI]
                              │
                    ┌─────────┴─────────┐
                    ▼                   ▼
              [Exit 1]            [Exit 2]
```

### 4.2 — Pro Mode with Tunnels

```
[Central] → [Tunnel 1] → [Tunnel 2] → ... → [Exit 1..6]
```

- Tunnel servers act as **relays only**
- Exit servers are the internet egress point (microsocks)
- **GRE fallback** activates when WireGuard fails

---

## 5. Operations Dashboard

### Basic Mode

<p align="center">
  <img src="assets/basic-dashboard.png" alt="Basic Dashboard" width="680">
</p>

### Pro Mode

<p align="center">
  <img src="assets/pro-operations.png" alt="Pro Dashboard" width="680">
</p>

---

## 6. Basic vs Pro

| Feature | Basic | Pro |
|---------|-------|-----|
| Target | Personal VPN | Commercial VPN |
| Recommended clicks | 3 | 6 |
| Exit servers | 1 + 2 | 1–6 |
| Tunnel servers | No | Yes |
| Domain / DNS | No | Yes |
| CDN | No | 6 providers |
| Free central countries | Iran, China, Russia | All countries |

<p align="center">
  <img src="assets/page-3-1.png" alt="Basic" width="280">
  <img src="assets/page-3-2.png" alt="Pro" width="280">
</p>

---

## 7. Core Technologies

| Layer | Technology |
|-------|------------|
| Client | Go + Fyne (Windows) |
| Tunnel | WireGuard (primary), GRE (fallback) |
| Panel | 3X-UI |
| Egress | microsocks |
| Transport | SSH with proxy support |
| Config | Local JSON |
| Updates | foxnext.net + blackfoxupdate.ir |
| Languages | 10 locales |

---

## 8. Security

- SSH authentication via password or key
- known_hosts to prevent MITM
- Machine-bound license (Machine ID)
- USDT payment verification via TX Hash
- SSH passwords never logged

---

## 9. Licensing Model

| Tier | Price | Network |
|------|-------|---------|
| Basic Full | 30 USDT | BEP-20 |
| Pro Full | 50 USDT | BEP-20 |

Activation methods: online (TX Hash), offline (BFXB/BFXP/BFXT codes), owner tool

---

## 10. Update Flow

The application uses two update servers:

1. `http://blackfoxupdate.ir` (primary)
2. `https://foxnext.net` (secondary)

Key files:

- `/version.json` — version and download URL
- `/news.json` — announcements
- `/wallet.json` — wallet address

---

## 11. Target Audience

- Personal users who want a private VPN panel
- Businesses needing multi-country VPN
- VPN service providers
- Server administrators with limited Linux experience

---

## 12. Links

| Resource | URL |
|----------|-----|
| Website | [foxnext.net](https://foxnext.net) |
| Download | [Setup.exe](https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe) |
| Telegram | [@blackFoxVPNN](https://t.me/blackFoxVPNN) |
| Roadmap | [ROADMAP.en.md](ROADMAP.en.md) |

---

© Black Fox Security Team — 2026
