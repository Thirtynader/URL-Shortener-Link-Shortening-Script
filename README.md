# 🔗 URL Shortener - Link Shortening Service

![URL Shortener](https://github.com/Thirtynader/URL-Shortener-Link-Shortening-Script/blob/main/Screenshotshorturl.png)

A modern, secure URL shortener with domain restrictions and beautiful starry UI design.

## ✨ Features

- 🔒 **Domain Restriction** - Only allows specific domains (default: 1hesekhob.com)
- ✏️ **Custom Slugs** - Choose your own short link name or get random
- 🔐 **Math CAPTCHA** - Security verification with math questions
- 📊 **Click Tracking** - Monitor link usage statistics
- 🎨 **Modern UI** - Beautiful starry background with light/dark theme
- 📱 **Responsive Design** - Works perfectly on all devices
- 🌍 **Multi-language Ready** - Default Persian, adaptable to any language

## 🎯 Live Demo

👉 [https://go.1hesekhob.com](https://go.1hesekhob.com)

## 💻 Requirements

- PHP 7.4 or higher
- Apache/Nginx with mod_rewrite
- Write permissions for links.json

## 🚀 Installation

1. Upload all files to your server
2. Ensure mod_rewrite is enabled
3. Set write permissions: `chmod 666 links.json`
4. Access your domain and start shortening!

## 📁 File Structure

```
├── index.html          # Main page
├── shorten.php         # URL shortening handler
├── redirect.php        # Redirect handler
├── .htaccess          # URL rewriting rules
└── links.json         # Links database (auto-created)
```

## 🔧 Configuration

### Change Allowed Domain

Edit `shorten.php` (line ~52):

```php
// Single domain
if (strpos($longUrl, 'yourdomain.com') === false) {

// Multiple domains
$allowedDomains = ['domain1.com', 'domain2.com'];
```

### Customize Slug Length

Edit `shorten.php` function `generateRandomSlug()`:

```php
function generateRandomSlug($length = 6) { // Change 6 to desired length
```

## 🔒 Security Features

- Math CAPTCHA verification
- Domain whitelist validation
- Input sanitization
- Slug validation (alphanumeric, dash, underscore only)

## 💰 Price

💲 Price: $10 | Lifetime Access | Free Updates

## 📧 Contact

For purchase or customization:
**Thirtynader@gmail.com**

## 📝 License

Copyright © 2013-2025 1hesekhob.com - Powered by Thirtynader

---

# 🔗 کوتاه کننده لینک - سرویس کوتاه‌سازی URL

یک کوتاه‌کننده لینک مدرن و امن با محدودیت دامنه و طراحی زیبای ستاره‌ای.

## ✨ امکانات

- 🔒 **محدودیت دامنه** - فقط دامنه‌های خاص (پیش‌فرض: 1hesekhob.com)
- ✏️ **نام دلخواه** - انتخاب نام سفارشی یا تصادفی
- 🔐 **کپچای ریاضی** - تأیید امنیتی با سوال ریاضی
- 📊 **شمارش کلیک** - رصد آمار استفاده از لینک
- 🎨 **رابط مدرن** - پس‌زمینه ستاره‌ای با حالت تاریک/روشن
- 📱 **طراحی ریسپانسیو** - کار با همه دستگاه‌ها
- 🌍 **چند زبانه** - پیش‌فرض فارسی، قابل ارائه به هر زبانی

## 🎯 دمو آنلاین

👉 [https://go.1hesekhob.com](https://go.1hesekhob.com)

## 💻 پیش‌نیازها

- PHP نسخه 7.4 یا بالاتر
- Apache/Nginx با mod_rewrite
- دسترسی نوشتن برای links.json

## 🚀 نصب

1. تمام فایل‌ها را روی سرور آپلود کنید
2. مطمئن شوید mod_rewrite فعال است
3. دسترسی نوشتن بدهید: `chmod 666 links.json`
4. به دامنه خود دسترسی پیدا کنید و شروع کنید!

## 📁 ساختار فایل‌ها

```
├── index.html          # صفحه اصلی
├── shorten.php         # هندلر کوتاه‌سازی
├── redirect.php        # هندلر ریدایرکت
├── .htaccess          # قوانین URL rewriting
└── links.json         # دیتابیس لینک‌ها (خودکار ساخته می‌شود)
```

## 🔧 تنظیمات

### تغییر دامنه مجاز

ویرایش `shorten.php` (خط 52):

```php
// یک دامنه
if (strpos($longUrl, 'yourdomain.com') === false) {

// چند دامنه
$allowedDomains = ['domain1.com', 'domain2.com'];
```

### تغییر طول کد تصادفی

ویرایش تابع `generateRandomSlug()` در `shorten.php`:

```php
function generateRandomSlug($length = 6) { // 6 را به طول دلخواه تغییر دهید
```

## 🔒 امکانات امنیتی

- تأیید کپچای ریاضی
- اعتبارسنجی دامنه مجاز
- پاکسازی ورودی‌ها
- اعتبارسنجی slug (فقط حروف، اعداد، خط تیره و زیرخط)

## 💰 قیمت

**10 دلار**

## 📧 تماس

برای خرید یا سفارشی‌سازی:
**Thirtynader@gmail.com**

## 📝 مجوز

کپی‌رایت © 2013-2025 1hesekhob.com - قدرت گرفته از Thirtynader
