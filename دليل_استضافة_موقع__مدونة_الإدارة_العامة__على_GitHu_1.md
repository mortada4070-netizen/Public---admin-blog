# دليل استضافة موقع "مدونة الإدارة العامة" على GitHub Pages

## الخطوة 1: إنشاء حساب GitHub

1. اذهب إلى موقع GitHub: https://github.com
2. اضغط على "Sign up" (إنشاء حساب)
3. أدخل بياناتك:
   - اسم المستخدم (Username): اختر اسمًا فريدًا
   - البريد الإلكتروني (Email)
   - كلمة المرور (Password)
4. أكمل عملية التحقق
5. اختر الخطة المجانية (Free)

## الخطوة 2: إنشاء مستودع جديد (Repository)

1. بعد تسجيل الدخول، اضغط على الزر الأخضر "New" أو علامة "+" في الأعلى
2. اختر "New repository"
3. أدخل اسم المستودع: `public-admin-blog`
4. تأكد من أن المستودع "Public" (عام)
5. ضع علامة ✓ على "Add a README file"
6. اضغط "Create repository"

## الخطوة 3: رفع ملفات الموقع

### الطريقة الأولى: عبر واجهة GitHub (الأسهل)

1. في صفحة المستودع الجديد، اضغط على "uploading an existing file"
2. اسحب وأفلت ملفات الموقع (الموجودة في الملف المضغوط الذي سأرسله لك)
3. أو اضغط "choose your files" واختر الملفات
4. في أسفل الصفحة، اكتب رسالة مثل "Add website files"
5. اضغط "Commit changes"

### الطريقة الثانية: عبر Git (للمتقدمين)

```bash
git clone https://github.com/[اسم-المستخدم]/public-admin-blog.git
cd public-admin-blog
# انسخ ملفات الموقع إلى هذا المجلد
git add .
git commit -m "Add website files"
git push origin main
```

## الخطوة 4: تفعيل GitHub Pages

1. في صفحة المستودع، اضغط على تبويب "Settings"
2. انتقل إلى قسم "Pages" في القائمة الجانبية
3. تحت "Source"، اختر "Deploy from a branch"
4. اختر "main" branch
5. اختر "/ (root)" folder
6. اضغط "Save"

## الخطوة 5: الحصول على رابط الموقع

بعد تفعيل GitHub Pages، ستحصل على رابط موقعك:
`https://[اسم-المستخدم].github.io/public-admin-blog`

## الخطوة 6: إضافة كود التحقق من Google Search Console

1. افتح ملف `index.html` في المستودع
2. اضغط على أيقونة القلم (Edit) لتحرير الملف
3. أضف كود التحقق من Google Search Console داخل قسم `<head>`:
   ```html
   <meta name="google-site-verification" content="G85Ytb5Gj1t2Hpxsdk3rT_phtPklQec2PeSfbdUgf6o" />
   ```
4. اضغط "Commit changes"

## الخطوة 7: إثبات الملكية في Google Search Console

1. عد إلى Google Search Console
2. أدخل رابط موقعك الجديد على GitHub Pages
3. اختر طريقة "HTML tag" للتحقق
4. تأكد من أن الكود موجود في ملف `index.html`
5. اضغط "Verify"

## ملاحظات مهمة:

- قد يستغرق الأمر بضع دقائق حتى يصبح موقعك متاحًا على GitHub Pages
- تأكد من أن جميع الملفات تم رفعها بنجاح
- إذا واجهت مشاكل، تحقق من أن اسم الملف الرئيسي هو `index.html` بالضبط
- GitHub Pages مجاني تمامًا للمستودعات العامة

