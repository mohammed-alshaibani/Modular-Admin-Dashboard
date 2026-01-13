# لوحة تحكم Laravel مع Tailwind CSS

## نظرة عامة
لوحة تحكم احترافية مبنية باستخدام Laravel 10 و Tailwind CSS 3. تحتوي على مجموعة غنية من المكونات الجاهزة للاستخدام مع واجهة مستخدم عصرية وسهلة التخصيص.

## المميزات الرئيسية

- **واجهة مستخدم حديثة** مع Tailwind CSS 3
- **مكونات حية** باستخدام Laravel Livewire 3
- **مصادقة جاهزة** مع Laravel Jetstream
- **واجهة برمجة التطبيقات (API)** مع Laravel Sanctum
- **تصميم متجاوب** يعمل على جميع الأجهزة
- **أداء عالي** مع Vite.js
- **مكونات تفاعلية** مع Alpine.js
- **رسوم بيانية** مع Chart.js
- **أيقونات SVG** متعددة الاستخدامات

## المتطلبات التقنية

- PHP 8.1 أو أحدث
- Composer
- Node.js 16.x أو أحدث
- قاعدة بيانات (MySQL 5.7+ / PostgreSQL / SQLite / SQL Server)
- NPM أو Yarn

## التثبيت

1. استنسخ المستودع:
   ```bash
   git clone [رابط المستودع]
   cd laravel-tailwindcss-admin-dashboard-template-main
   ```

2. قم بتثبيت حزم PHP:
   ```bash
   composer install
   ```

3. قم بإنشاء ملف `.env` من الملف النموذجي:
   ```bash
   cp .env.example .env
   ```

4. قم بإنشاء مفتاح التطبيق:
   ```bash
   php artisan key:generate
   ```

5. قم بتكوين إعدادات قاعدة البيانات في ملف `.env`:
   ```env
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=اسم_قاعدة_البيانات
   DB_USERNAME=اسم_المستخدم
   DB_PASSWORD=كلمة_المرور
   ```

6. قم بتشغيل الهجرات وبذر البيانات:
   ```bash
   php artisan migrate --seed
   ```

7. قم بتثبيت حزم Node.js:
   ```bash
   npm install
   ```

8. قم ببناء الأصول:
   ```bash
   npm run dev
   # أو للبيئة الإنتاجية
   npm run build
   ```

9. قم بتشغيل خادم التطوير:
   ```bash
   php artisan serve
   ```

## بيانات الدخول الافتراضية

- **البريد الإلكتروني:** admin@example.com
- **كلمة المرور:** password

## هيكل المشروع

```
├── app/                # ملفات التطبيق
├── bootstrap/          # ملفات تمهيد Laravel
├── config/             # ملفات التكوين
├── database/           # الهجرات والنماذج
├── public/             # الملفات العامة
├── resources/          # الموارد (العروض، الترجمة، الأصول)
│   ├── css/            # أنماط CSS
│   ├── js/             # سكريبتات JavaScript
│   └── views/          # قوالب Blade
├── routes/             # مسارات التطبيق
└── tests/              # الاختبارات
```

## التخصيص

### تغيير الألوان
يمكنك تخصيص الألوان من خلال تعديل ملف `tailwind.config.js`:

```javascript
module.exports = {
  theme: {
    extend: {
      colors: {
        primary: {
          DEFAULT: '#4F46E5',
          // ...
        }
      }
    }
  }
}.
