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
  <a href="https://foxnext.net/en/privacy.html">Privacy Policy</a> •
  <a href="https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe">Black Fox Vpn-Installer-Setup.exe</a> •
  <a href="https://foxnext.net/downloads/BlackFox-VPN-Android-release.apk">BlackFox-VPN-Android-release.apk</a> •
  <a href="https://foxnext.net/downloads/Black-Fox-Config-Builder.apk">Black-Fox-Config-Builder.apk</a> •
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
- Move Central Server (Windows + Android)  
- License Reactivation after reinstall  
- Backup / restore during Central Server migration  
- Companion **Black Fox Config Builder** for 3X-UI config creation on Android  

The suite is designed for networks with restricted global access and helps operators deploy multi-location VPN infrastructure without deep Linux expertise.

### Current releases

| Platform | Product | Status | Download |
|----------|---------|--------|----------|
| Windows | **Black Fox Vpn Installer** v1.3.0 (Build 202) | Available | [Black Fox Vpn-Installer-Setup.exe](https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe) |
| Android | **BlackFox Vpn Android** v0.4.13 (Build 21) | Available | [BlackFox-VPN-Android-release.apk](https://foxnext.net/downloads/BlackFox-VPN-Android-release.apk) |
| Android | **Black Fox Config Builder** v1.1.3 (Build 7) | Available | [Black-Fox-Config-Builder.apk](https://foxnext.net/downloads/Black-Fox-Config-Builder.apk) |
| Android | Google Play listing | **Coming Soon** | — |
| macOS | Black Fox Vpn | **Coming Soon** | — |

> **BlackFox Vpn Android** is released and available from the official website. Google Play publication is **Coming Soon**.

---

## 2. Features

- Automated 3X-UI (Sanaei) installation and panel configuration  
- WireGuard primary tunnels + GRE fallback  
- Basic Mode and Pro Mode  
- Central / Tunnel / Exit server operations  
- Domain & subdomain management (Pro)  
- CDN automation on Windows Pro  
- **Move Central Server on Windows and Android (Pro)** with automated panel-client transfer  
- **License Reactivation** after app reinstall on the same device (Registration → Reactivation)  
- Dual update hosts (`foxnext.net` + `blackfoxupdate.ir`)  
- Companion **Black Fox Config Builder** for phone-side 3X-UI config creation  
- Official website + Privacy Policy  

<p align="center">
  <img src="docs/assets/page-0.png" alt="Basic Mode vs Pro Mode" width="520">
</p>

---

## 3. Basic Mode

Basic Mode is for operators who need a simpler and faster structure:

- Central Server Setup  
- Connect SSH / Full Deploy  
- Exit servers (slots 1–2)  
- Configure Panel  
- Core helpers (Install WireGuard / Install 3X-UI)  

<p align="center">
  <img src="docs/assets/dashboard-basic.png" alt="Black Fox Vpn Installer — Basic Mode dashboard" width="520">
</p>

---

## 4. Pro Mode

Pro Mode is for advanced multi-server infrastructure:

- Central Server  
- Tunnel Server  
- Exit Server (up to 6)  
- WireGuard + GRE  
- Domain / DNS management  
- CDN providers (Windows Pro)  
- **Move Central Server (Windows + Android)**  
- Migration backup + automated panel client continuity  

<p align="center">
  <img src="docs/assets/dashboard-pro.png" alt="Black Fox Vpn Installer — Pro Mode dashboard" width="520">
</p>

### Move Central Server

Using **Move Central Server**, relocating the central role no longer requires a full manual rebuild.

Enter the new central server details and the operation runs automatically:

- Tunnel servers and exit servers are reconnected to the new central  
- 3X-UI panel client configuration is transferred automatically  
- Local migration backup is created during the process  

Available in **Pro Mode on both Windows and Android**.

---

## 5. License Reactivation (important update)

Latest licensing workflow no longer requires users to permanently keep offline license codes for normal reinstall cases.

On the **Registration** screen:

1. Reinstall the app on the **same device**  
2. Open Registration  
3. Press **Reactivation** / **فعال‌سازی مجدد**  

The app checks the previous activation record bound to that device’s machine fingerprint and restores access when the record is valid.

Notes:

- Reactivation works for previously activated devices recorded by the official activation service  
- Online TX verification and offline codes remain available as alternative paths  
- Reactivation is designed so users do not need to store license codes only to recover after uninstall/reinstall on the same device  

---

## 6. Android Version

**BlackFox Vpn Android is released.**

| Item | Value |
|------|-------|
| Product name | BlackFox Vpn Android |
| Version | 0.4.13 (Build 21) |
| Download file | [BlackFox-VPN-Android-release.apk](https://foxnext.net/downloads/BlackFox-VPN-Android-release.apk) |
| Google Play | **Coming Soon** |

Android Pro Mode includes **Move Central Server** and **License Reactivation**, alongside Basic/Pro operations for Central / Tunnel / Exit management.

<p align="center">
  <img src="docs/assets/android-dashboard.png" alt="BlackFox Vpn Android" width="48%">
  &nbsp;
  <img src="docs/assets/android-vpn/choose-mode-duo.png" alt="Choose Mode" width="48%">
</p>

<p align="center">
  <img src="docs/assets/android-vpn/basic-mode-duo.png" alt="Android Basic" width="32%">
  <img src="docs/assets/android-vpn/pro-mode-duo.png" alt="Android Pro" width="32%">
  <img src="docs/assets/android-config-builder.png" alt="Black Fox Config Builder" width="32%">
</p>

---

## 7. Black Fox Config Builder (Android companion)

**Black Fox Config Builder** is a separate Android companion for creating 3X-UI client configs from the phone. It is **not** a VPN client and **not** a server deployer.

| Item | Value |
|------|-------|
| Full product name | Black Fox Config Builder |
| Version | 1.1.3 (Build 7) |
| Package ID | `com.blackfoxvpnn.configbuilder` |
| Download file | [Black-Fox-Config-Builder.apk](https://foxnext.net/downloads/Black-Fox-Config-Builder.apk) |
| Dedicated GitHub docs | [balckfoxgroup/blackfox-config-builder](https://github.com/balckfoxgroup/blackfox-config-builder) |
| Min Android | API 24 (Android 7.0+) |
| Required panel | 3X-UI **3.3.0 or newer** |

### What it does

1. Connect to an existing 3X-UI panel using credentials from **Panel Login Info** in Black Fox Vpn Installer / BlackFox Vpn Android  
2. Create **single** configs (name / random name, traffic, duration, **multi-inbound**, VLESS + Subscription links, QR codes)  
3. Create **bulk** configs with progress and stop  
4. Manage a local **List** — copy link, **delete from panel**, delete from list  
5. **Settings** — 10 languages, dual-server update check (`blackfoxupdate.ir` + `foxnext.net`), force update, activity log  
6. **Contact** — website, email, GitHub, Telegram accounts  

Build 6 introduced the dual-server remote feed. Build 7 is the current published Android release with the full six-tab workflow above.

---

## 8. Windows Version

| Item | Value |
|------|-------|
| Product name | Black Fox Vpn Installer |
| Version | 1.3.0 (Build 202) |
| Download file | [Black Fox Vpn-Installer-Setup.exe](https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe) |

Windows remains the full desktop operations console for Basic and Pro workflows, including CDN automation and Move Central Server.

---

## 9. Supported Languages

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

Coverage includes Black Fox Vpn Installer, BlackFox Vpn Android, Black Fox Config Builder, and the website at [foxnext.net](https://foxnext.net).

---

## 10. Architecture

```text
Central Server
      ↓
Tunnel Server
      ↓
Exit Server
      ↓
Client Infrastructure
```

The application simplifies installation, configuration, migration, and day-to-day management of this chain.

---

## 11. WireGuard and GRE

- **WireGuard** is the primary tunnel technology  
- **GRE** is available as a fallback path when WireGuard cannot sustain the route  
- Exit servers provide egress; tunnel servers act as relays in Pro Mode  

---

## 12. Central / Tunnel / Exit Servers

| Role | Purpose |
|------|---------|
| Central Server | Hub with 3X-UI panel and orchestration point |
| Tunnel Server | Optional Pro multi-hop relay |
| Exit Server | Internet egress location |

Basic Mode focuses on Central + limited Exit slots. Pro Mode adds Tunnel servers, expanded Exit capacity, Domain/CDN (Windows), and Move Central Server (Windows + Android).

---

## 13. Domain Management

In Pro Mode, operators can manage domains/subdomains with DNS automation.

Current DNS providers include:

- Cloudflare  
- ArvanCloud  

Windows Pro also includes CDN operations for:

- ArvanCloud  
- Cloudflare  
- KeyCDN  
- Other CDN  

---

## 14. Privacy Policy

A dedicated Privacy Policy is published on the official website:

- English: [https://foxnext.net/en/privacy.html](https://foxnext.net/en/privacy.html)  
- Persian: [https://foxnext.net/fa/privacy.html](https://foxnext.net/fa/privacy.html)  

Please treat those pages as the authoritative privacy source.

---

## 15. Roadmap & Whitepaper

- Roadmap EN: [docs/ROADMAP.en.md](docs/ROADMAP.en.md)  
- Roadmap FA: [docs/ROADMAP.fa.md](docs/ROADMAP.fa.md)  
- Whitepaper EN: [docs/WHITEPAPER.en.md](docs/WHITEPAPER.en.md)  
- Whitepaper FA: [docs/WHITEPAPER.fa.md](docs/WHITEPAPER.fa.md)  

| Status | Examples |
|--------|----------|
| Completed | Windows + Android releases, Move Central (Win+Android), License Reactivation, Black Fox Config Builder Build 7, 10 languages, Basic/Pro, WireGuard/GRE |
| In Progress | UX hardening, Android/Windows parity improvements |
| Planned | macOS, Google Play listing, broader standalone Backup/Restore tooling, mid-workflow resume UI |

---

## 16. Support the Project

If BlackFox VPN Installer is useful to you, please support Black Fox Group development by starring the repository.

- Star the Repository  
- Report Bugs  
- Suggest Features  
- Share the Project  
- Support the Development  

Channels:

- Telegram: [https://t.me/blackFoxVPNN](https://t.me/blackFoxVPNN)  
- Website: [https://foxnext.net](https://foxnext.net)  
- GitHub: [https://github.com/balckfoxgroup/blackfox-vpn-installer](https://github.com/balckfoxgroup/blackfox-vpn-installer)  
- Email: support@foxnext.net  

---

## 17. License

Commercial product. Basic / Pro licensing is managed through official registration flows on [foxnext.net](https://foxnext.net).

Current public website pricing: Basic **19 USDT** · Pro **33 USDT** (confirm on site).

---

# فارسی

## ۱. معرفی پروژه

**Black Fox Vpn Installer** یک کلاینت VPN ساده نیست.

این مجموعه، ابزارهای **مدیریت و راه‌اندازی سرور** برای این حوزه‌هاست:

- اتوماسیون استقرار سرور  
- مدیریت زیرساخت چندسروری  
- پیکربندی زیرساخت VPN  
- مدیریت Central Server  
- مدیریت Tunnel Server  
- مدیریت Exit Server  
- انتقال Central Server (ویندوز و اندروید)  
- فعال‌سازی مجدد لایسنس پس از نصب مجدد  
- بکاپ و بازیابی در مسیر انتقال سرور مرکزی  
- ابزار همراه **Black Fox Config Builder** برای ساخت کانفیگ 3X-UI روی اندروید  

این نرم‌افزار برای شرایطی طراحی شده که دسترسی به اینترنت جهانی محدود است و به شما کمک می‌کند بدون دانش عمیق لینوکس، زیرساخت VPN چندلوکیشن خود را راه‌اندازی و مدیریت کنید.

### وضعیت انتشار فعلی

| پلتفرم | محصول | وضعیت | دانلود |
|--------|--------|--------|--------|
| ویندوز | **Black Fox Vpn Installer** نسخه 1.3.0 (Build 202) | منتشر شده | [Black Fox Vpn-Installer-Setup.exe](https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe) |
| اندروید | **BlackFox Vpn Android** نسخه 0.4.13 (Build 21) | منتشر شده | [BlackFox-VPN-Android-release.apk](https://foxnext.net/downloads/BlackFox-VPN-Android-release.apk) |
| اندروید | **Black Fox Config Builder** نسخه 1.1.3 (Build 7) | منتشر شده | [Black-Fox-Config-Builder.apk](https://foxnext.net/downloads/Black-Fox-Config-Builder.apk) |
| اندروید | انتشار در Google Play | **به‌زودی (Coming Soon)** | — |
| macOS | Black Fox Vpn | **به‌زودی** | — |

> نسخه Android برنامه BlackFox منتشر شده است و کاربران می‌توانند آن را از وب‌سایت رسمی Black Fox Group دانلود کنند. نسخه Android به‌زودی در Google Play نیز منتشر خواهد شد.

---

## ۲. امکانات

- نصب و پیکربندی خودکار پنل 3X-UI (سنایی)  
- تونل WireGuard به‌همراه GRE fallback  
- حالت‌های Basic و Pro  
- عملیات Central / Tunnel / Exit  
- مدیریت Domain و Subdomain در Pro  
- اتوماسیون CDN در Pro ویندوز  
- **Move Central Server روی ویندوز و اندروید (Pro)** با انتقال خودکار کلاینت‌های پنل  
- **فعال‌سازی مجدد لایسنس** پس از حذف و نصب مجدد روی همان دستگاه  
- دو میزبان آپدیت: `foxnext.net` و `blackfoxupdate.ir`  
- ابزار همراه **Black Fox Config Builder** برای ساخت کانفیگ 3X-UI از روی گوشی  
- وب‌سایت رسمی و صفحه حریم خصوصی  

---

## ۳. Basic Mode

برای کاربرانی که به ساختار ساده‌تر و سریع‌تر نیاز دارند:

- راه‌اندازی Central Server  
- اتصال SSH و Full Deploy  
- سرورهای Exit (اسلات ۱ و ۲)  
- Configure Panel  
- ابزارهای کمکی نصب WireGuard و 3X-UI  

---

## ۴. Pro Mode

برای مدیریت زیرساخت‌های پیشرفته و چندسروری:

- Central Server  
- Tunnel Server  
- Exit Server (تا ۶ خروجی)  
- WireGuard و GRE  
- مدیریت Domain / DNS  
- CDN (در نسخه ویندوز)  
- **Move Central Server در ویندوز و اندروید**  
- بکاپ مسیر انتقال و حفظ تداوم کلاینت‌های پنل  

### انتقال Central Server

با کلید **Move Central Server** دیگر لازم نیست انتقال سرور مرکزی را دستی و از صفر انجام دهید.

اطلاعات سرور مرکزی جدید را وارد کنید؛ عملیات به‌صورت خودکار اجرا می‌شود:

- تمام Tunnel Serverها و Exit Serverها به مرکزی جدید متصل می‌شوند  
- پیکربندی کلاینت‌های پنل 3X-UI به‌صورت خودکار منتقل می‌شود  
- در مسیر انتقال، بکاپ محلی ساخته می‌شود  

این قابلیت در **Pro Mode ویندوز و اندروید** فعال است.

---

## ۵. فعال‌سازی مجدد لایسنس (تغییر مهم)

در آخرین تغییرات نوع فعال‌سازی لایسنس، دیگر لازم نیست کاربر کد لایسنس را برای حالت عادی نصب مجدد دائماً نگهداری کند.

روی صفحه **ثبت‌نام / Registration**:

۱. برنامه را روی **همان دستگاه** دوباره نصب کنید  
۲. وارد تب ثبت‌نام شوید  
۳. فقط دکمه **فعال‌سازی مجدد (Reactivation)** را بزنید  

برنامه سابقه فعال‌سازی همان دستگاه را از سرویس رسمی بررسی می‌کند و در صورت معتبر بودن، دسترسی را بازیابی می‌کند.

نکته‌ها:

- این مسیر برای دستگاهی کار می‌کند که قبلاً فعال شده و رکورد آن در سرویس فعال‌سازی ثبت شده باشد  
- مسیرهای پرداخت آنلاین (TX Hash) و کد آفلاین همچنان به‌عنوان روش‌های جایگزین باقی هستند  
- هدف این است که کاربر برای بازیابی پس از حذف/نصب مجدد، مجبور به نگهداری دائمی کد لایسنس نباشد  

---

## ۶. نسخه اندروید

| مورد | مقدار |
|------|--------|
| نام کامل محصول | BlackFox Vpn Android |
| نسخه | 0.4.13 (Build 21) |
| فایل دانلود | [BlackFox-VPN-Android-release.apk](https://foxnext.net/downloads/BlackFox-VPN-Android-release.apk) |
| Google Play | **به‌زودی** |

در نسخه اندروید، علاوه بر عملیات Basic/Pro، قابلیت‌های **Move Central Server** و **فعال‌سازی مجدد لایسنس** نیز فعال هستند.

---

## ۷. Black Fox Config Builder (ابزار همراه اندروید)

**Black Fox Config Builder** یک برنامه جداگانه اندروید برای ساخت کانفیگ کلاینت روی پنل 3X-UI از طریق گوشی است. این برنامه **کلاینت VPN** نیست و **نصب‌کننده سرور** هم نیست.

| مورد | مقدار |
|------|--------|
| نام کامل محصول | Black Fox Config Builder |
| نسخه | 1.1.3 (Build 7) |
| شناسه بسته | `com.blackfoxvpnn.configbuilder` |
| فایل دانلود | [Black-Fox-Config-Builder.apk](https://foxnext.net/downloads/Black-Fox-Config-Builder.apk) |
| مستندات جداگانه گیت‌هاب | [balckfoxgroup/blackfox-config-builder](https://github.com/balckfoxgroup/blackfox-config-builder) |
| حداقل اندروید | API 24 (اندروید ۷ به بالا) |
| پنل موردنیاز | 3X-UI نسخه **۳.۳.۰ یا جدیدتر** |

### این برنامه چه می‌کند

۱. اتصال به پنل 3X-UI موجود با اطلاعات **Panel Login Info** از Black Fox Vpn Installer یا BlackFox Vpn Android  
۲. ساخت کانفیگ **تکی** (نام یا نام تصادفی، حجم، مدت، **انتخاب چند Inbound**، لینک VLESS و Subscription، QR Code)  
۳. ساخت کانفیگ **گروهی** با نوار پیشرفت و امکان توقف  
۴. مدیریت **لیست** محلی — کپی لینک، **حذف از پنل**، حذف از لیست  
۵. **تنظیمات** — ۱۰ زبان، بررسی آپدیت از دو سرور (`blackfoxupdate.ir` و `foxnext.net`)، Force Update، لاگ فعالیت  
۶. **تماس** — وب‌سایت، ایمیل، گیت‌هاب و حساب‌های تلگرام  

Build 6 فید ریموت دو سرور را معرفی کرد. Build 7 نسخه فعلی منتشرشده اندروید با گردش‌کار کامل شش تب بالاست.

---

## ۸. نسخه ویندوز

| مورد | مقدار |
|------|--------|
| نام کامل محصول | Black Fox Vpn Installer |
| نسخه | 1.3.0 (Build 202) |
| فایل دانلود | [Black Fox Vpn-Installer-Setup.exe](https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe) |

---

## ۹. پشتیبانی از ۱۰ زبان

محصولات Black Fox Group برای مخاطب بین‌المللی طراحی شده‌اند و از ۱۰ زبان زنده دنیا پشتیبانی می‌کنند:

انگلیسی، فارسی، روسی، چینی، آلمانی، ازبکی، ترکی، اندونزیایی، اوکراینی و هندی.

این پوشش شامل Black Fox Vpn Installer، BlackFox Vpn Android، Black Fox Config Builder و وب‌سایت [foxnext.net](https://foxnext.net) است.

---

## ۱۰. معماری

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

## ۱۱. حریم خصوصی

سیاست حریم خصوصی به‌صورت جداگانه منتشر شده است:

- فارسی: [https://foxnext.net/fa/privacy.html](https://foxnext.net/fa/privacy.html)  
- انگلیسی: [https://foxnext.net/en/privacy.html](https://foxnext.net/en/privacy.html)  

---

## ۱۲. نقشه راه و وایت‌پیپر

- [docs/ROADMAP.fa.md](docs/ROADMAP.fa.md)  
- [docs/WHITEPAPER.fa.md](docs/WHITEPAPER.fa.md)  
- [docs/ROADMAP.en.md](docs/ROADMAP.en.md)  
- [docs/WHITEPAPER.en.md](docs/WHITEPAPER.en.md)  

---

## ۱۳. حمایت از پروژه

اگر BlackFox VPN Installer برای شما مفید است، با دادن یک Star به Repository از توسعه Black Fox Group حمایت کنید.

- Star the Repository  
- Report Bugs  
- Suggest Features  
- Share the Project  
- Support the Development  

- تلگرام: [https://t.me/blackFoxVPNN](https://t.me/blackFoxVPNN)  
- وب‌سایت: [https://foxnext.net](https://foxnext.net)  
- گیت‌هاب: [https://github.com/balckfoxgroup/blackfox-vpn-installer](https://github.com/balckfoxgroup/blackfox-vpn-installer)  
- ایمیل: support@foxnext.net  

---

© Black Fox Security Team
