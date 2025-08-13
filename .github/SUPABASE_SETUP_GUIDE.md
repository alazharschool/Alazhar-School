# دليل إعداد Supabase لمشروع Al-Azhar School

## 🎯 الخطوات المطلوبة

### 1. إنشاء حساب Supabase
- اذهب إلى [https://supabase.com](https://supabase.com)
- اضغط "Start your project" 
- سجل دخول بحساب GitHub أو Google

### 2. إنشاء مشروع جديد
- اضغط "New Project"
- اختر اسم للمشروع: `al-azhar-school`
- اختر كلمة مرور قوية لقاعدة البيانات
- اختر المنطقة الأقرب لك (مثل Europe West)
- انتظر حتى يكتمل الإعداد (5-10 دقائق)

### 3. الحصول على معلومات الاتصال
بعد اكتمال المشروع، اذهب إلى:
- **Settings** → **API**
- انسخ:
  - `Project URL` 
  - `anon public` key

### 4. تطبيق قاعدة البيانات
- اذهب إلى **SQL Editor**
- انسخ محتوى ملف `supabase-schema.sql`
- اضغط "Run" لتطبيق الجداول

### 5. تحديث ملف البيئة
أضف المعلومات في ملف `.env.local`:
```env
NEXT_PUBLIC_SUPABASE_URL=YOUR_ACTUAL_SUPABASE_URL
NEXT_PUBLIC_SUPABASE_ANON_KEY=YOUR_ACTUAL_ANON_KEY
NEXT_PUBLIC_SITE_URL=http://localhost:3000
```

### 6. اختبار الاتصال
- أعد تشغيل السيرفر
- جرب تسجيل دخول جديد
- تحقق من إنشاء المستخدمين في قاعدة البيانات

## ⚠️ ملاحظات مهمة
- لا تشارك مفاتيح API مع أي شخص
- استخدم Row Level Security (RLS) للأمان
- احتفظ بنسخة احتياطية من قاعدة البيانات

## 🔧 استكشاف الأخطاء
إذا واجهت مشاكل:
1. تحقق من صحة URL و API Key
2. تأكد من تطبيق schema قاعدة البيانات
3. تحقق من إعدادات RLS
4. راجع سجلات الأخطاء في Supabase
