# Lootlo Android App - Starter Project

Yeh Android Studio/Gradle project ka starter hai. Yeh Lootlo website ko Android WebView ke andar kholta hai, back navigation, loading indicator, offline screen aur external links handling deta hai.

## Zaroori baat
- Is project ko yahan compile/test nahi kiya gaya hai.
- Yeh APK/AAB file nahi, balki source project hai.
- Play Store approval guaranteed nahi hai. Google Play minimal-functionality policy ke kaaran sirf website-wrapper app reject ho sakti hai.
- Payment/checkout, login, uploads aur external payment redirects ko real device par test karna zaroori hai.
- Play Store publishing ke liye signed AAB aur privacy policy chahiye.

## Sirf Android phone se build karne ka raasta
1. ZIP ko download aur extract karein.
2. GitHub account banayein/sign in karein: https://github.com
3. Naya repository banayein, jaise `lootlo-android`.
4. Extract kiye gaye project ke sab files repository mein upload karein (folders ki structure same rakhein).
5. GitHub mein `Actions` tab kholein aur Android Build workflow run karein. Push par bhi workflow automatically chalega.
6. Build successful hone par workflow run ke neeche `Artifacts` mein `lootlo-debug-apk` download karein.
7. Yeh debug APK testing ke liye hai, Play Store release ke liye nahi.

## Play Store release
Play Store ke liye signed release AAB, keystore/signing configuration, privacy policy, store listing aur Play Console account chahiye. Keystore/password ko public GitHub repository mein kabhi upload na karein. Production release se pehle Android developer ki madad se signing aur policy compliance verify karna recommended hai.

## Website
Default URL: https://lootlo.co.in
Agar domain/checkout flow badalta hai, `app/src/main/java/in/lootlo/app/MainActivity.kt` mein `START_URL` update karein.
