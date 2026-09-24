# Toe Pwar Gyi — APK Build (မြန်မာ)

ဒီ project က Android APK build လုပ်ရန် ပြင်ထားတဲ့ project ဖြစ်ပါတယ်။

## GitHub နဲ့ APK ထုတ်နည်း (Android ဖုန်းကနေပါ လုပ်နိုင်)

1. GitHub account ဝင်ပါ။
2. Repository အသစ်တစ်ခုဖန်တီးပါ — ဥပမာ `toe-pwar-gyi-app`။
3. ဒီ project folder ထဲက files အားလုံးကို repository ထဲ Upload files လုပ်ပါ။ `.github/workflows/build-apk.yml` ကိုပါ upload လုပ်ရပါမယ်။
4. Upload ပြီးရင် **Actions** tab ကိုဖွင့်ပါ။
5. **Build Toe Pwar Gyi APK** workflow ကိုရွေးပါ။
6. **Run workflow** ကိုနှိပ်ပါ။
7. Build ပြီးရင် workflow ရဲ့ **Artifacts** အောက်မှာ `ToePwarGyi-debug-apk` ကို Download လုပ်ပါ။
8. ZIP ဖြည်ပြီး `app-debug.apk` ကို Android ဖုန်းထဲ Install လုပ်ပါ။

## Android ဖုန်းမှာ Install

APK ကို Download ပြီး ဖွင့်ပါ။ Android က Unknown app install permission တောင်းရင် browser/file manager အတွက် **Allow from this source** ကိုဖွင့်ပြီး Install လုပ်ပါ။

## မှတ်ချက်

- ဒီ build က debug APK ဖြစ်ပါတယ်။ Play Store တင်ရန် signed release AAB/APK ထပ် build လုပ်ရပါမယ်။
- Firebase/Leaflet CDN features တွေအတွက် Internet permission ပါပါတယ်။
- GPS အတွက် Fine/Coarse location permission ပါပါတယ်။
- Background GPS tracking (screen ပိတ်ပြီး ဆက်ပို့ခြင်း) မပါသေးပါ။
