# BlackFox VPN Android

اپلیکیشن موبایل **BlackFox VPN Android**.

مسیر Flutter: `Mobile/flutter/`  
موتور Go: `mobile/` (gomobile → `mobile.aar`)

## نصب یک‌جا

### ۱. Flutter SDK

```powershell
.\Mobile\scripts\setup-flutter.ps1
```

در صورت خطای دانلود Dart، با VPN نصب کنید.

### ۲. Android Studio

- Android SDK
- یک Emulator یا گوشی با USB debugging

متغیر محیطی:

```
ANDROID_HOME=C:\Users\YOU\AppData\Local\Android\Sdk
```

### ۳. کتابخانه Go (استقرار واقعی)

```powershell
.\Mobile\scripts\build-gomobile.ps1
```

خروجی: `Mobile/flutter/android/app/libs/mobile.aar`

بدون این فایل، اپ فقط تست SSH با Dart را انجام می‌دهد.

## اجرا

```powershell
cd Mobile\flutter
flutter pub get
flutter run
```

## ساخت APK (یک‌جا)

```powershell
.\Mobile\scripts\build-release.ps1
```

خروجی نهایی (فقط در این پوشه):

```
Mobile\App Bundle\BlackFox-VPN-Android-release.apk
```

برای Google Play و APKهای جداگانه هر ABI:

```powershell
.\Mobile\scripts\build-play-bundle.ps1
```

```
Mobile\App Bundle\BlackFox-VPN-Android-release.aab
Mobile\App Bundle\BlackFox-VPN-Android-arm64-v8a-release.apk
Mobile\App Bundle\BlackFox-VPN-Android-armeabi-v7a-release.apk
Mobile\App Bundle\BlackFox-VPN-Android-x86_64-release.apk
```

Keystore release (خودکار در اولین بیلد):

```
Mobile\BlackFox-VPN-Android-release\blackfox-vpn-release.jks
Mobile\flutter\android\key.properties
```

رمزها در `Mobile\BlackFox-VPN-Android-release\KEYSTORE-CREDENTIALS.local.txt` ذخیره می‌شوند (commit نشود).

اسکریپت بالا SDK، NDK، `mobile.aar` و APK امضا‌شده release را می‌سازد (برای ایران از آینه Tencent/Aliyun استفاده می‌کند).

### ساخت دستی

```powershell
.\Mobile\scripts\install-android-sdk.ps1
.\Mobile\scripts\build-gomobile.ps1
cd Mobile\flutter
flutter pub get
flutter build apk --release
```

خروجی Gradle: `build\app\outputs\flutter-apk\app-release.apk`

```powershell
adb install Mobile\App Bundle\BlackFox-VPN-Android-release.apk
```

**حجم APK:** حدود ۵۴۵ مگابایت (به‌خاطر موتور Go و بسته‌های embedded 3X-UI داخل `mobile.aar`).

## تست موتور Go روی ویندوز (بدون اندروید)

```powershell
go run -tags has3xui ./cmd/mobile-test -host VPS_IP -user root -pass SECRET -tcp
go run -tags has3xui ./cmd/mobile-test -host VPS_IP -user root -pass SECRET
```

## معماری (۰.۳.۰)

```
Flutter UI
  └─ MethodChannel com.blackfoxvpnn.android/engine
       └─ BlackfoxEngineHandler.kt (reflection)
            └─ mobile.aar (Go: mobile/engine.go)
                 └─ deploy.Orchestrator → WireGuard + Sanaei
```

**Fallback:** اگر `mobile.aar` نباشد → `dartssh2` برای تست SSH.

## قابلیت‌ها (۰.۴.۱۳ / Build 21)

| قابلیت | وضعیت |
|--------|--------|
| تم + ۱۰ زبان + RTL | آماده |
| Basic / Pro (بدون CDN) | آماده |
| سرور مرکزی + پروکسی | آماده |
| Full Deploy (Go) | نیاز به `mobile.aar` |
| سرور خروجی ۱ و ۲+ | آماده (Go) |
| تونل Pro | آماده (Go) |
| افزودن دامنه (بدون CDN) | آماده |
| **Move Central Server (Pro)** | آماده (Go + Flutter) |
| ثبت‌نام / TX / کد آفلاین | آماده (Go) |
| **فعال‌سازی مجدد لایسنس (Reactivation)** | آماده — پس از حذف/نصب مجدد روی همان دستگاه، فقط یک کلید |
| حذف سرورها / بازنشانی | آماده (Go) |

دانلود رسمی:

- [BlackFox-VPN-Android-release.apk](https://foxnext.net/downloads/BlackFox-VPN-Android-release.apk)

## نام برنامه

در UI و اندروید: **BlackFox VPN Android**