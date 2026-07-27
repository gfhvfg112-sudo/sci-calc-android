# ماشین حساب مهندسی (Android)

پروژه‌ی کامل اندروید (Kotlin + Gradle KTS). موتور محاسبات و رابط کاربری در `app/src/main/assets/index.html` است و کاملاً آفلاین اجرا می‌شود (هیچ مجوز اینترنتی درخواست نمی‌شود).

## قابلیت‌ها
- توابع مثلثاتی sin/cos/tan و معکوس‌های آن‌ها، حالت DEG/RAD
- ln، log، توان (x^y)، مربع، جذر، ریشه سوم، معکوس (1/x)
- فاکتوریل، باقیمانده (mod)، درصد، نماد علمی (EE)
- ثابت‌های π و e، پرانتز تودرتو، ضرب ضمنی مانند 2(3+4)
- حافطه MC / M+ / MR و تاریخچه‌ی ۲۰ محاسبه‌ی اخیر
- ارزیاب عبارت با الگوریتم shunting-yard، بدون استفاده از eval

## بیلد APK روی GitHub Actions
ورک‌فلوی `.github/workflows/build.yml` با هر push روی `main` اجرا می‌شود و `SciCalc.apk` را در بخش Releases منتشر می‌کند.

## بیلد محلی
```bash
# JDK 17 و Android SDK لازم است
gradle wrapper
./gradlew assembleDebug
# خروجی: app/build/outputs/apk/debug/app-debug.apk
```
