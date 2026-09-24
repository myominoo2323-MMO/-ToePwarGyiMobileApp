# Toe Pwar Gyi Business Mobile App v20

ပါဝင်မှုများ
- Orders / Sales / Customers / Products / Cars / Reports / Backup
- Firebase Authentication Login
- Firestore businessData/main cloud sync
- Firebase Realtime Database vehicleLocations real-time GPS
- Leaflet + OpenStreetMap Live Vehicles Map
- CAR-01 ... CAR-05
- Android WebView mobile application wrapper

## Android Studio
1. Folder `ToePwarGyiMobileApp` ကို Android Studio နဲ့ Open လုပ်ပါ။
2. Gradle Sync လုပ်ပါ။
3. Android phone ကို USB debugging ဖြင့်ချိတ်ပါ။
4. Run လုပ်ပါ။

## Firebase
Web app config ကို HTML ထဲမှာထည့်ပြီးသားဖြစ်ပါတယ်။ Firebase Console မှာ:
- Authentication > Email/Password enabled
- Firestore Database created
- Realtime Database created
- Existing users collection / rules ကိုသုံးပါ

Business cloud data path:
`businessData/main`

GPS path:
`vehicleLocations/CAR-01` ... `CAR-05`

## Important
ဒီ version က Android app ဖွင့်ထားပြီး GPS tracking စထားချိန်မှာ real-time GPS ပို့နိုင်ပါတယ်။ Screen ပိတ်ထားချိန်/Background မှာ ဆက်လက် GPS ပို့ရန် native Android Foreground Location Service ကို နောက်ထပ်ထည့်ရပါမယ်။

## Production
Play Store release အတွက် applicationId, icon, signing key, privacy policy, Firebase security rules hardening, background-location compliance စတာတွေကို production မတင်မီ ပြင်ဆင်ရပါမယ်။


## Installable App (PWA)
- `app/src/main/assets/manifest.webmanifest` and `sw.js` are included.
- When the HTML is hosted over HTTPS, Chrome/Edge can install it as an app on Android and Windows/macOS.
- The app still needs internet access for Firebase and OpenStreetMap tiles.
- True background GPS while the screen is locked requires a native Android foreground-location service; the current WebView layer does not implement that service yet.

## Android APK build
This source is Android Studio/Gradle-ready, but a compiled APK is not produced in this environment because the Android SDK/Gradle build toolchain is not installed here.
