# نقشه راه — Black Fox Vpn Installer

**نسخه:** 1.3.0 | **Build:** 202 | **به‌روزرسانی:** ژوئیه ۲۰۲۶

[English version](ROADMAP.en.md)

---

## چشم‌انداز

ارائه ساده‌ترین مسیر برای راه‌اندازی و مدیریت زیرساخت VPN چندلوکیشن روی سرورهای لینوکس — بدون نیاز به دانش عمیق لینوکس.

محصولات Black Fox Group **مجموعه ابزارهای مدیریت و راه‌اندازی سرور** هستند، نه یک کلاینت VPN ساده.

<p align="center">
  <img src="assets/page-0.png" alt="Basic Mode در برابر Pro Mode" width="640">
</p>

---

## راهنمای وضعیت

| برچسب | معنا |
|-------|------|
| **Completed** | منتشر شده و در محصول فعلی موجود است |
| **In Progress** | در حال بهبود فعال |
| **Planned** | در نقشه راه؛ هنوز قابلیت نهایی منتشرشده نیست |

---

## Completed (تکمیل‌شده)

| مورد | توضیح |
|------|--------|
| انتشار ویندوز — Black Fox Vpn Installer | v1.3.0 (Build 202) |
| انتشار اندروید — BlackFox Vpn Android | v0.4.13 (Build 21) |
| Black Fox Config Builder (اندروید) | v1.1.3 (Build 7) |
| پشتیبانی از ۱۰ زبان (اپ + وب‌سایت) | انگلیسی، فارسی، روسی، چینی، آلمانی، ازبکی، ترکی، اندونزیایی، اوکراینی، هندی |
| Basic Mode | جریان ساده‌تر Central + Exit |
| Pro Mode | عملیات زیرساخت چندسروری |
| مدیریت Central Server | Setup، SSH، Full Deploy، نصب پنل |
| مدیریت Tunnel Server (Pro) | زنجیره رله چند hop |
| مدیریت Exit Server | Basic: ۱–۲ · Pro: ۱–۶ |
| پشتیبانی WireGuard | مسیر اصلی تونل |
| پشتیبانی GRE fallback | وقتی مسیر WireGuard قطع می‌شود |
| مدیریت Domain و Subdomain (Pro) | Cloudflare و ArvanCloud |
| اتوماسیون CDN (Pro، ویندوز) | ArvanCloud، Cloudflare، KeyCDN، Other CDN |
| نصب و مدیریت خودکار 3X-UI (سنایی) | بسته embed + پیکربندی پنل |
| انتقال Central Server (Pro) | مهاجرت زیرساخت با انتقال خودکار کلاینت‌های پنل |
| بکاپ محلی هنگام Move Central | اسنپ‌شات در مسیر انتقال |
| پروکسی هوشمند SSH | برای شبکه‌های محدود |
| دو میزبان آپدیت | `foxnext.net` و `blackfoxupdate.ir` |
| ثبت لایسنس USDT | سطوح Basic / Pro |
| وب‌سایت رسمی | [foxnext.net](https://foxnext.net) |
| صفحه Privacy Policy | [فارسی](https://foxnext.net/fa/privacy.html) · [انگلیسی](https://foxnext.net/en/privacy.html) |

---

## In Progress (در حال توسعه)

| مورد | توضیح |
|------|--------|
| بهبود تجربه Basic Mode | وضعیت واضح‌تر و جریان‌های راهنما |
| بهبود تجربه Pro Mode | شفافیت عملیات و مسیرهای حذف/ریست امن‌تر |
| هم‌ترازی ترجمه‌های ۱۰ زبانه | اپ‌ها و وب‌سایت |
| نزدیک‌کردن قابلیت‌های اندروید به Pro ویندوز | CDN و برخی عملیات پیشرفته هنوز اولویت ویندوز دارند |
| پایداری تحویل روی هاست‌ها | آپلود/آپدیت پایدارتر |

---

## Planned (برنامه‌های آینده)

| مورد | توضیح |
|------|--------|
| نسخه macOS | به‌زودی |
| انتشار در Google Play برای اندروید | **Coming Soon** (دانلود APK از وب‌سایت هم‌اکنون فعال است) |
| ادامه Workflow از مراحل میانی | UI امن‌تر برای ادامه از checkpoint |
| Backup و Restore مستقل زیرساخت | فراتر از اسنپ‌شات Move Central |
| زنجیره تونل طولانی‌تر | مقیاس‌پذیری multi-hop |
| گزارش ترافیک و uptime | دید عملیاتی |
| Remote management API | کنترل برنامه‌ای |
| ربات تلگرام | کمک عملیاتی آینده |

---

## ماتریس پلتفرم

| پلتفرم | محصول | وضعیت |
|--------|--------|--------|
| Windows | Black Fox Vpn Installer | **Available** — v1.3.0 (Build 202) |
| Android | BlackFox Vpn Android | **Available** — v0.4.13 (Build 21) |
| Android | Black Fox Config Builder | **Available** — v1.1.3 (Build 7) |
| Android | انتشار Google Play | **Coming Soon** |
| macOS | Black Fox Vpn | **Coming Soon** |

---

## Basic در برابر Pro (وضعیت فعلی)

<p align="center">
  <img src="assets/dashboard-basic.png" alt="داشبورد Basic" width="360">
  &nbsp;
  <img src="assets/dashboard-pro.png" alt="داشبورد Pro" width="360">
</p>

| قابلیت | Basic | Pro |
|--------|-------|-----|
| Central Server | بله | بله |
| Exit Servers | ۱–۲ | ۱–۶ |
| Tunnel Servers | خیر | بله |
| Domain / DNS | خیر | بله |
| CDN | خیر | بله (ویندوز) |
| Move Central Server | خیر | بله |
| WireGuard + GRE | بله | بله |

---

## لینک‌ها

- وب‌سایت: [foxnext.net](https://foxnext.net)
- حریم خصوصی: [foxnext.net/fa/privacy.html](https://foxnext.net/fa/privacy.html)
- دانلود ویندوز / اندروید / Config Builder از وب‌سایت رسمی
- تلگرام: [@blackFoxVPNN](https://t.me/blackFoxVPNN)
- مخزن: [balckfoxgroup/blackfox-vpn-installer](https://github.com/balckfoxgroup/blackfox-vpn-installer)

---

## Support the Project

اگر BlackFox VPN Installer برای شما مفید است، با دادن یک Star به Repository از توسعه Black Fox Group حمایت کنید.

- Star the Repository
- Report Bugs
- Suggest Features
- Share the Project
- Support the Development

© Black Fox Security Team
