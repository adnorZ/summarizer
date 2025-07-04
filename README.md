YouTube Video Summarizer Extension
ملخص فيديوهات اليوتيوب - إضافة متصفح كروم لتلخيص فيديوهات اليوتيوب تلقائياً باستخدام الذكاء الاصطناعي.
Show Image
✨ المميزات الرئيسية
🎯 تلخيص ذكي

استخراج تلقائي للنصوص المرفقة مع الفيديو
تلخيص دقيق باستخدام OpenAI GPT
دعم اللغتين العربية والإنجليزية
خيارات طول الملخص (موجز/مفصل)

🔧 سهولة الاستخدام

واجهة بسيطة وسلسة
زر تلخيص مباشر أسفل الفيديو
تلخيص تلقائي عند تحميل الفيديو (اختياري)
حفظ وتصدير الملخصات

📊 إدارة البيانات

حفظ الملخصات محلياً
تصدير الملخصات بصيغة JSON أو Markdown
إحصائيات مفصلة عن الاستخدام
تنظيف تلقائي للبيانات القديمة

🚀 التثبيت والإعداد
المتطلبات الأساسية

متصفح Google Chrome أو أي متصفح يدعم Chromium
مفتاح OpenAI API (احصل عليه من هنا)

خطوات التثبيت
تفعيل وضع المطور في كروم

افتح Chrome واذهب إلى chrome://extensions/
فعّل "Developer mode" من الزاوية العلوية اليمنى
اضغط على "Load unpacked"
اختر مجلد الإضافة


إعداد مفتاح API

اضغط على أيقونة الإضافة في شريط المتصفح
أدخل مفتاح OpenAI API في الإعدادات
احفظ الإعدادات


بدء الاستخدام

اذهب إلى أي فيديو يوتيوب
ستظهر واجهة التلخيص تلقائياً
اضغط على "تلخيص الفيديو"



📋 هيكل الملفات
youtube-summarizer-extension/
├── manifest.json          # إعدادات الإضافة الأساسية
├── content.js            # سكريبت المحتوى الرئيسي
├── background.js         # سكريبت الخلفية
├── popup.html           # واجهة الإعدادات
├── popup.js             # منطق الإعدادات
├── styles.css           # تنسيقات الإضافة
├── icons/               # أيقونات الإضافة
│   ├── icon16.png
│   ├── icon48.png
│   └── icon128.png
└── README.md           # هذا الملف
⚙️ التكوين المتقدم
إعدادات API
javascript// في popup.js - يمكن تخصيص هذه القيم
const API_SETTINGS = {
  openai: {
    baseUrl: 'https://api.openai.com/v1',
    model: 'gpt-3.5-turbo',
