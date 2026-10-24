# MoPlayer Native — النسخة 7
1. ارفع كل محتويات المجلد على مستودع GitHub (استبدل القديم).
2. Actions ← Build APK ← نزّل MoPlayer-APK وثبّته.

## الجديد في النسخة 7
- واجهة جديدة بألوان وأيقونات التصميم (هيدر، تبويبات، أزرار أناشيد / القرآن الكريم / أخرى).
- تصنيف تلقائي لكل ملف: قرآن أو أنشودة أو أخرى (من الاسم واسم الملف والفنان والألبوم والنوع والمجلد). تقدر تنقل أي ملف يدوي من أيقونة الترس.
- آخر حاجة اتشغلت بتظهر تحت دايمًا (حتى بعد قفل التطبيق) وبتكمل من نفس المكان.
- الواجهة بتتكيف مع حجم الشاشة: تليفون، تابلت، لابتوب (أعمدة أكتر ومشغّل أفقي).


## توضيح نوع المشروع والتعديلات
- هذا مشروع أندرويد أصلي مكتوب بـ Kotlin وJetpack Compose، وليس صفحة HTML أو WebView.
- يحتوي على ملفات Gradle وAndroidManifest ومصدر التطبيق وموارد الخطوط وأيقونات التطبيق.
- شريط الساعة والبطارية والشبكة هو شريط نظام أندرويد، ولا يتم رسم نسخة مزيفة منه داخل الواجهة.
- تم ضبط أيقونة القوائم لتكون أيقونة موسيقى/قوائم، مع إظهار موجات متحركة للملف الجاري تشغيله والملفات المحددة.
- لا يعني ملف ZIP أنه APK جاهز للتثبيت؛ هو أرشيف ملفات المشروع المصدر. يجب فتح المجلد في Android Studio أو تشغيل بناء Gradle لإنتاج APK.
- المطابقة البكسلية التامة للصورة غير مضمونة لأن النصوص ومحتوى المكتبة وحجم الشاشة وحالة التشغيل تختلف على الجهاز؛ التصميم مستوحى من الصورة مع الحفاظ على الوظائف الأصلية.


## Home track-row refinements
- Audio rows now show square album artwork on the right in the Arabic (RTL) layout.
- If no embedded/album artwork is available, the same square displays a centered “M” logo; real artwork replaces the logo automatically.
- Track title spacing from the artwork has been increased.
- The currently playing row shows animated audio bars next to its title, animated while playback is active and settled while paused.
- The open/chevron indicator is on the left side of the row.
