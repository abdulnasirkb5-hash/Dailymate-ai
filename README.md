# DailyMate AI — hybrid starter version 0.2

A responsive installable web-app prototype and starting point for an Android app. It is designed to keep its core tools usable offline after the first successful load.

## Included
- Mobile-friendly home screen and English, Arabic, Urdu and Hindi header/interface selector
- Offline message/email draft templates
- Common phrase examples in four languages (not a general-purpose translation engine)
- CV profile builder
- Social caption templates
- Percentage, discount and bill-split calculator
- Quick notes saved locally on the device
- Online/offline connection indicator
- Service-worker caching for repeat/offline access
- Premium and advertising placeholders

## What requires a later online service integration
- Real AI writing, rewriting and CV generation
- Full sentence translation
- Cloud accounts and sync
- AdMob advertising and premium subscriptions

Do not put a private AI API key inside the app. A production AI integration should call a secure backend that protects the key and applies usage limits.

## Run locally
Serve this folder from localhost or HTTPS (service workers require a secure context):

```bash
python -m http.server 8000
```

Open http://localhost:8000. For offline testing, open the app once while online, then disconnect and reload.

## Android packaging
This is a PWA prototype, not a compiled APK. To create an Android APK/AAB, wrap it with a native Android shell (for example Capacitor), configure a unique application ID, icons, permissions and signing, then build and test using Android Studio and the Android SDK.
