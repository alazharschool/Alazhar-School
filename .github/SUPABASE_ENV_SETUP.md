# 🔧 تحديث ملف .env.local

## ⚠️ مهم: هذا الملف محمي من التعديل التلقائي

يجب عليك تحديث ملف `.env.local` يدوياً بالمعلومات الصحيحة من Supabase.

## 📝 الخطوات:

### 1. فتح ملف .env.local
```bash
# في Windows
notepad .env.local

# أو في أي محرر نصوص
code .env.local
```

### 2. استبدال القيم التالية:

**قبل التعديل:**
```env
NEXT_PUBLIC_SUPABASE_URL=YOUR_SUPABASE_URL
NEXT_PUBLIC_SUPABASE_ANON_KEY=YOUR_SUPABASE_ANON_KEY
```

**بعد التعديل:**
```env
NEXT_PUBLIC_SUPABASE_URL=https://abcdefghijklm.supabase.co
NEXT_PUBLIC_SUPABASE_ANON_KEY=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
```

## 🔑 كيفية الحصول على المعلومات:

1. **اذهب إلى [https://supabase.com](https://supabase.com)**
2. **سجل دخول أو أنشئ حساب جديد**
3. **أنشئ مشروع جديد:**
   - اسم المشروع: `al-azhar-school`
   - كلمة مرور قوية لقاعدة البيانات
   - اختر المنطقة الأقرب لك
4. **انتظر حتى يكتمل الإعداد (5-10 دقائق)**
5. **اذهب إلى Settings → API**
6. **انسخ:**
   - `Project URL`
   - `anon public` key

## ✅ بعد التحديث:

1. **احفظ الملف**
2. **أعد تشغيل السيرفر:**
   ```bash
   npm run dev
   ```
3. **جرب تسجيل دخول جديد**
4. **تحقق من إنشاء المستخدمين في قاعدة البيانات**

## 🆘 إذا واجهت مشاكل:

- تأكد من صحة URL و API Key
- تأكد من تطبيق schema قاعدة البيانات في Supabase
- تحقق من إعدادات Row Level Security (RLS)
- راجع سجلات الأخطاء في Supabase
