# وایت‌پیپر — Black Fox Vpn Installer

**نسخه:** 1.3.0 | **Build:** 200 | **به‌روزرسانی:** ژوئیه ۲۰۲۶

[English version](WHITEPAPER.en.md)

---

## ۱. خلاصه اجرایی

**Black Fox Vpn Installer** یک کلاینت VPN ساده نیست.

این محصول **مجموعه ابزارهای مدیریت و راه‌اندازی سرور** برای موارد زیر است:

- Server Deployment Automation  
- Multi-Server Infrastructure Management  
- VPN Infrastructure Configuration  
- Central Server Management  
- Tunnel Management  
- Exit Server Management  
- Backup and Restore (در مسیر انتقال Central Server)  

خانواده محصول هم‌اکنون روی **ویندوز** و **اندروید** منتشر شده و ابزار **Config Builder** اندروید نیز در دسترس است. نسخه **macOS** در برنامه است. انتشار در **Google Play** برای اندروید به‌صورت **Coming Soon** اعلام می‌شود؛ دانلود APK از وب‌سایت رسمی فعال است.

وب‌سایت رسمی: [https://foxnext.net](https://foxnext.net)

---

## ۲. صورت‌مسئله

راه‌اندازی زیرساخت VPN چندلوکیشن معمولاً نیازمند این کارهاست:

- نصب دستی WireGuard و مسیریابی  
- راه‌اندازی پنل 3X-UI  
- مدیریت SSH، فایروال و اعتبارنامه‌ها  
- اتصال سرورهای خروجی به هاب مرکزی  
- در صورت نیاز، اتوماسیون CDN / DNS  

برای اپراتورهایی که دانش عمیق لینوکس ندارند، این مسیر زمان‌بر و خطاپذیر است.

---

## ۳. راه‌حل

برنامه‌های Black Fox Group عملیات پیچیده چندسروری را به جریان‌های گرافیکی قابل‌هدایت تبدیل می‌کنند.

از ویندوز یا اندروید می‌توان این موارد را نصب و مدیریت کرد:

- پنل 3X-UI (سنایی)  
- WireGuard  
- توپولوژی Exit و Tunnel  
- اتوماسیون Domain / CDN (Pro)  
- انتقال Central Server با حفظ تداوم کلاینت‌ها  

<p align="center">
  <img src="assets/page-0.png" alt="نمای Basic و Pro" width="650">
</p>

---

## ۴. معماری

زنجیره کلی:

```text
Central Server
      ↓
Tunnel Server (Pro، اختیاری)
      ↓
Exit Server
      ↓
Client Infrastructure
```

### ۴.۱ Basic Mode

برای ساختار ساده‌تر و سریع‌تر:

- Central Server  
- Exit محدود  
- Configure Panel  

### ۴.۲ Pro Mode

برای زیرساخت پیشرفته چندسروری:

- Central / Tunnel / Exit  
- WireGuard + GRE  
- Domain و CDN  
- Move Central Server  

<p align="center">
  <img src="assets/dashboard-basic.png" alt="داشبورد Basic" width="420">
  &nbsp;
  <img src="assets/dashboard-pro.png" alt="داشبورد Pro" width="420">
</p>

---

## ۵. انتشار پلتفرم‌ها

| پلتفرم | محصول | وضعیت |
|--------|--------|--------|
| Windows | Black Fox Vpn Installer v1.3.0 (Build 200) | Available |
| Android | BlackFox Vpn Android v0.4.13 (Build 20) | Available از وب‌سایت |
| Android | Google Play | **Coming Soon** |
| Android | Config Builder v1.1.3 (Build 7) | Available |
| macOS | Black Fox Vpn | Coming Soon |

<p align="center">
  <img src="assets/android-dashboard.png" alt="نسخه اندروید" width="520">
</p>

> نسخه Android برنامه BlackFox منتشر شده است و کاربران می‌توانند آن را از وب‌سایت رسمی Black Fox Group دانلود کنند. نسخه Android به‌زودی در Google Play نیز منتشر خواهد شد.

---

## ۶. پشتیبانی از ۱۰ زبان

محصولات Black Fox Group برای مخاطب بین‌المللی طراحی شده‌اند و از **۱۰ زبان زنده دنیا** پشتیبانی می‌کنند:

انگلیسی، فارسی، روسی، چینی، آلمانی، ازبکی، ترکی، اندونزیایی، اوکراینی و هندی.

---

## ۷. Domain، CDN و انتقال Central

- DNS: Cloudflare و ArvanCloud  
- CDN (ویندوز Pro): ArvanCloud، Cloudflare، KeyCDN، Other CDN  
- Move Central Server: بکاپ مسیر انتقال + انتقال خودکار کلاینت‌های پنل با هدف حفظ دسترسی  

Backup/Restore گسترده‌تر به‌عنوان ابزار مستقل در نقشه راه باقی است.

---

## ۸. حریم خصوصی (Privacy Policy)

سیاست حریم خصوصی به‌صورت جداگانه منتشر شده است:

- فارسی: [https://foxnext.net/fa/privacy.html](https://foxnext.net/fa/privacy.html)  
- انگلیسی: [https://foxnext.net/en/privacy.html](https://foxnext.net/en/privacy.html)  

کاربران می‌توانند جزئیات مرتبط با داده و حریم خصوصی را در همان صفحه رسمی مطالعه کنند.

---

## ۹. امنیت و لایسنس

- احراز هویت SSH با رمز یا کلید  
- لایسنس وابسته به دستگاه  
- عدم ثبت رمزها در لاگ برنامه  
- سطوح Basic / Pro با جریان USDT (قیمت به‌روز را در وب‌سایت ببینید)

---

## ۱۰. لینک‌ها

| منبع | آدرس |
|------|------|
| وب‌سایت | [foxnext.net](https://foxnext.net) |
| حریم خصوصی | [foxnext.net/fa/privacy.html](https://foxnext.net/fa/privacy.html) |
| دانلود ویندوز | [Setup.exe](https://foxnext.net/downloads/Black%20Fox%20Vpn-Installer-Setup.exe) |
| دانلود اندروید | [APK](https://foxnext.net/downloads/BlackFox-VPN-Android-release.apk) |
| Config Builder | [GitHub](https://github.com/balckfoxgroup/blackfox-config-builder) |
| تلگرام | [@blackFoxVPNN](https://t.me/blackFoxVPNN) |
| نقشه راه | [ROADMAP.fa.md](ROADMAP.fa.md) |

---

## Support the Project

اگر BlackFox VPN Installer برای شما مفید است، با دادن یک Star به Repository از توسعه Black Fox Group حمایت کنید.

- Star the Repository  
- Report Bugs  
- Suggest Features  
- Share the Project  
- Support the Development  

© Black Fox Security Team — ۲۰۲۶
