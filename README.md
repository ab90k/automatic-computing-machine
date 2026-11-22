# أموالي — مشروع تطبيق أندرويد

## بناء ملف APK

### الطريقة 1: Android Studio (الأسهل)
1. ثبّت Android Studio من developer.android.com/studio
2. File ← Open ← اختر مجلد المشروع (Amwali) وانتظر انتهاء المزامنة
3. Build ← Build Bundle(s) / APK(s) ← Build APK(s)
4. تلاقي الملف في: app/build/outputs/apk/debug/app-debug.apk

### الطريقة 2: GitHub Actions (بدون تثبيت شي)
1. ارفع محتوى المجلد على مستودع GitHub جديد
2. افتح تبويب Actions ← Build APK ← Run workflow
3. بعد انتهاء البناء نزّل الملف من Artifacts (amwali-apk)

### التثبيت
انقل app-debug.apk للموبايل وافتحه (فعّل «التثبيت من مصادر غير معروفة» إذا طلب).
لنسخة النشر على Google Play: Build ← Generate Signed Bundle / APK.

## الملفات
- app/src/main/assets/index.html : واجهة التطبيق كاملة
- MainActivity.kt : غلاف WebView + البصمة + الحفظ والمشاركة
