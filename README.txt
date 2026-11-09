موقع ابن حميدو — طريقة التشغيل

الملفات:
- index.html: الموقع كامل بالمنيو والعروض والأرقام والأزرار.
- firebase-config.js: إعدادات Firebase المطلوبة للتقييمات المشتركة.
- firestore.rules: قواعد قاعدة البيانات.

مهم: الموقع يشتغل كصفحة عادية بعد رفعه، لكن التقييمات لن تُحفظ وتظهر لكل الزوار إلا بعد إعداد Firebase.

إعداد التقييمات المشتركة:
1) افتح https://console.firebase.google.com/ وأنشئ مشروعًا جديدًا.
2) من Build افتح Firestore Database ثم Create database.
3) من Project Overview اضغط علامة الويب </> لإضافة Web App.
4) انسخ إعدادات SDK التي تظهر لك وضع القيم الحقيقية في firebase-config.js بدل YOUR_API_KEY وYOUR_PROJECT_ID وغيرها.
5) افتح Firestore Database > Rules، والصق محتوى firestore.rules ثم اضغط Publish.

رفع الموقع:
1) افتح مستودع GitHub.
2) ارفع index.html وfirebase-config.js (واستبدل الملفات القديمة إذا طُلب).
3) اعمل Commit changes وانتظر تحديث GitHub Pages.
ملف firestore.rules مرجع لنسخ القواعد داخل Firebase فقط، وليس مطلوبًا تشغيله من الموقع.

روابط أُضيفت:
Bio: https://bio.site/mohamedali1
خريطة المطعم: https://maps.app.goo.gl/micxmJHBBgMpH31F9

ملاحظات:
- لم يصلني رابط جروب واتساب، لذلك لم أضع رابطًا غير مؤكد. أرسل الرابط لإضافته.
- الأسعار وأرقام الهاتف والعروض مأخوذة من الكود الذي أرسلته؛ راجعها قبل النشر.
- قواعد Firestore تسمح للزوار بالقراءة والإضافة فقط، وتمنع التعديل والحذف. لكنها لا تمنع الرسائل المزعجة بالكامل؛ فعّل Firebase App Check قبل نشر الموقع على نطاق واسع.
- لا تضع Service Account key أو مفاتيح Admin في ملفات الموقع.
