# indo

[![GitHub Repo stars](https://img.shields.io/github/stars/hishamalmushrea-cloud/indo?style=social)](https://github.com/hishamalmushrea-cloud/indo)
[![GitHub](https://img.shields.io/github/license/hishamalmushrea-cloud/indo)](https://github.com/hishamalmushrea-cloud/indo/blob/main/LICENSE)
[![Trendshift](https://trendshift.io/api/badge/repositories/4119)](https://trendshift.io/)
[![Docs Website](https://img.shields.io/badge/Docs-Website-blue?style=for-the-badge&logo=readthedocs)](https://github.com/hishamalmushrea-cloud/indo)
[![Discord](https://img.shields.io/badge/Discord-Join%20Us-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com/)
[![X (formerly Twitter) Follow](https://img.shields.io/twitter/follow/hishamalmushrea-cloud?style=social)](https://x.com/hishamalmushrea-cloud)

---

# IndoLearn - تعلم اللغة الإندونيسية

تطبيق Android كامل واحترافي لتعليم اللغة الإندونيسية للناطقين بالعربية من الصفر إلى المستوى المتوسط.

## المميزات المكتملة

- 14 شاشة حقيقية تعمل
- Text-to-Speech (نطق إندونيسي) + سرعات مختلفة
- اختبارات تفاعلية مع نتائج
- نظام Flashcards
- **مدرب الإندونيسية اليومية** (قسم كبير ومتكامل)
  - 40+ تعبير يومي حقيقي مع تصنيف الرسمية
  - 4 سيناريوهات واقعية (سوق، مطعم، شارع، محل)
  - تمارين متعددة (استماع، ترجمة، ترتيب كلمات، موقف)
  - نظام تدريب تفاعلي
- بحث متقدم
- مفضلة + تقدم المستخدم
- مراجعة يومية
- محادثات وقواعد حقيقية
- إشعارات يومية
- دعم الوضع الداكن + RTL
- قاعدة بيانات Room محلية (Offline 100%)

## كيفية فتح المشروع

1. افتح **Android Studio** (Hedgehog أو أحدث)
2. `File → Open`
3. اختر المجلد الرئيسي
4. انتظر Gradle Sync
5. اضغط **Run**

## بناء التطبيق

```bash
# داخل Android Studio:
Build → Build Bundle(s) / APK(s) → Build APK(s)
```

سيتم إنشاء `app-debug.apk` في:
`app/build/outputs/apk/debug/`

## هيكل المشروع

```
app/
├── data/
│   ├── local/          # Room + Entities + DAOs
│   └── repository/
├── ui/
│   ├── screens/        # جميع الشاشات
│   └── theme/
├── utils/              # TTS + Notifications
├── navigation/
└── viewmodel/
```

## إضافة محتوى جديد

يمكنك إضافة دروس أو مفردات جديدة داخل `LearnRepository.seedInitialData()`.

## الترخيص

مشروع تعليمي مفتوح المصدر.

---

**تم تطوير التطبيق بالكامل باستخدام Kotlin + Jetpack Compose + Room + MVVM**