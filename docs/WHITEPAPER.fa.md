<p align="right">
  <img src="assets/logo.jpg" alt="Black Fox VPN" width="120" align="left">
</p>

# وایت‌پیپر — Black Fox Vpn Installer

**نسخه:** 1.3.0 | **Build:** 194

[English version](WHITEPAPER.en.md)

---

## ۱. خلاصه اجرایی

**Black Fox Vpn Installer** یک برنامه ویندوزی تجاری است که با اتصال SSH به سرورهای لینوکس، زیرساخت VPN چندلوکیشنی را به‌صورت خودکار راه‌اندازی می‌کند.

کاربر بدون دانش تخصصی لینوکس می‌تواند:

- سرور مرکزی با پنل 3X-UI نصب کند
- سرورهای خروجی در کشورهای مختلف اضافه کند
- در مد Pro، زنجیره تونل relay بسازد
- CDN و DNS را پیکربندی کند

---

## ۲. مسئله

راه‌اندازی VPN چندلوکیشنی معمولاً نیازمند:

- نصب دستی WireGuard
- پیکربندی پنل 3X-UI
- مدیریت SSH و فایروال
- اتصال سرورهای خارجی به سرور مرکزی

این فرآیند برای کاربران غیرفنی زمان‌بر و پرخطاست.

---

## ۳. راه‌حل

برنامه تمام مراحل را در یک داشبورد گرافیکی یکپارچه می‌کند:

```
Initial Server Setup → Connect SSH → Full Deploy → Exit Servers → Configure Panel
```

<p align="center">
  <img src="assets/page-0.png" alt="معماری Basic و Pro" width="650">
</p>

---

## ۴. معماری شبکه

### ۴.۱ — حالت Basic

```
[کاربر ویندوز] → SSH → [سرور مرکزی: WireGuard + 3X-UI]
                              │
                    ┌─────────┴─────────┐
                    ▼                   ▼
              [خروجی ۱]           [خروجی ۲]
```

### ۴.۲ — حالت Pro با تونل

```
[سرور مرکزی] → [تونل ۱] → [تونل ۲] → ... → [خروجی ۱..۶]
```

- سرورهای تونل فقط **relay** هستند
- سرور خروجی نقطه خروج اینترنت است (microsocks)
- در صورت شکست WireGuard، **GRE fallback** فعال می‌شود

---

## ۵. داشبورد Operations

### Basic Mode

<p align="center">
  <img src="assets/basic-dashboard.png" alt="Basic Dashboard" width="680">
</p>

### Pro Mode

<p align="center">
  <img src="assets/pro-operations.png" alt="Pro Dashboard" width="680">
</p>

---

## ۶. مد Basic و Pro

| ویژگی | Basic | Pro |
|-------|-------|-----|
| هدف | VPN شخصی | VPN تجاری |
| کلیک پیشنهادی | ۳ | ۶ |
| سرور خروجی | ۱ + ۲ | ۱ تا ۶ |
| سرور تونل | ندارد | دارد |
| دامنه / DNS | ندارد | دارد |
| CDN | ندارد | ۶ ارائه‌دهنده |
| کشور رایگان مرکزی | ایران، چین، روسیه | همه کشورها |

<p align="center">
  <img src="assets/page-3-1.png" alt="Basic" width="280">
  <img src="assets/page-3-2.png" alt="Pro" width="280">
</p>

---

## ۷. فناوری‌های اصلی

| لایه | فناوری |
|------|--------|
| کلاینت | Go + Fyne (Windows) |
| تونل | WireGuard (اصلی), GRE (جایگزین) |
| پنل | 3X-UI |
| خروجی | microsocks |
| ارتباط | SSH با پشتیبانی پروکسی |
| تنظیمات | JSON محلی |
| آپدیت | foxnext.net + blackfoxupdate.ir |
| زبان | ۱۰ زبان |

---

## ۸. امنیت

- اتصال SSH با احراز هویت رمز یا کلید
- known_hosts برای جلوگیری از MITM
- لایسنس ماشین‌بند (Machine ID)
- تأیید پرداخت USDT از طریق TX Hash
- بدون ذخیره رمز SSH در لاگ

---

## ۹. مدل لایسنس

| سطح | قیمت | شبکه |
|-----|------|------|
| Basic Full | ۳۰ USDT | BEP-20 |
| Pro Full | ۵۰ USDT | BEP-20 |

روش‌های فعال‌سازی: آنلاین (TX Hash)، آفلاین (کد BFXB/BFXP/BFXT)، ابزار مالک

---

## ۱۰. جریان آپدیت

برنامه از دو سرور آپدیت استفاده می‌کند:

1. `http://blackfoxupdate.ir` (اصلی)
2. `https://foxnext.net` (ثانویه)

فایل‌های کلیدی:

- `/version.json` — نسخه و لینک دانلود
- `/news.json` — اخبار
- `/wallet.json` — آدرس کیف پول

---

## ۱۱. مخاطبان هدف

- کاربران شخصی که VPN اختصاصی می‌خواهند
- کسب‌وکارهایی که VPN چندکشوری نیاز دارند
- ارائه‌دهندگان خدمات VPN
- مدیران سرور با دانش محدود لینوکس

---

## ۱۲. لینک‌ها

| منبع | آدرس |
|------|------|
| وب‌سایت | [foxnext.net](https://foxnext.net) |
| دانلود | [Setup.exe](https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe) |
| تلگرام | [@blackFoxVPNN](https://t.me/blackFoxVPNN) |
| نقشه راه | [ROADMAP.fa.md](ROADMAP.fa.md) |

---

© Black Fox Security Team — 2026
