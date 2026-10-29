# 🏆 ChampZone - Complete Esports Android App Project

यह ChampZone Esports Tournament ऐप का पूरा सोर्स कोड और प्रोजेक्ट गाइड है।

---

## 📥 ZIP फाइल सीधे अपनी स्क्रीन से डाउनलोड कैसे करें:

### विकल्प A: AI Studio के टॉप बार से Direct 1-Click Export (सबसे तेज़)
1. अपनी स्क्रीन के **ऊपर दाईं तरफ (Top-Right)** देखें।
2. वहाँ आपको **Share** बटन के पास **"Export"** या **तीन डॉट्स (⋮)** / **Settings ⚙️** का आइकन दिखेगा।
3. उस पर क्लिक करें और **"Download ZIP"** या **"Export as ZIP"** चुनें।
4. आपके ब्राउज़र में पूरा प्रोजेक्ट (`ChampZone.zip`) तुरंत डाउनलोड होना शुरू हो जाएगा!

### विकल्प B: APK बनाकर सीधे फोन में इंस्टॉल करना
1. उसी टॉप मेन्यू (Settings ⚙️) में जाएँ।
2. **"Generate APK"** चुनें।
3. कुछ ही पलों में रेडी-टू-इंस्टॉल APK डाउनलोड हो जाएगी, जिसे आप सीधे अपने Android फोन में इनस्टॉल कर सकते हैं।

---

## 📁 प्रोजेक्ट स्ट्रक्चर (What's Inside the ZIP):

```
ChampZone/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/
│   │   │   │   ├── MainActivity.kt                  # Main Host Activity & Navigation Host
│   │   │   │   ├── ui/
│   │   │   │   │   ├── screens/
│   │   │   │   │   │   ├── HomeDashboardScreen.kt   # White theme Dashboard, live countdown & matches
│   │   │   │   │   │   ├── PhoneAuthScreen.kt       # Phone + OTP (SMS/WhatsApp/Call) + Name signup
│   │   │   │   │   │   ├── AdminScreen.kt           # Admin batch schedule, 15% host share, Bank/UPI
│   │   │   │   │   │   ├── MatchDetailScreen.kt     # Match rules, prize calculator, slot map
│   │   │   │   │   │   ├── WalletScreen.kt          # UPI deposit, withdrawal, balance card
│   │   │   │   │   │   ├── ProfileScreen.kt         # KYC, Free Fire/BGMI UID, virus scanner
│   │   │   │   │   │   ├── MyMatchesScreen.kt       # Joined matches, credentials countdown
│   │   │   │   │   │   ├── RewardsScreen.kt         # Esports coins, redeem rewards
│   │   │   │   │   │   └── TournamentsListScreen.kt # Filterable tournament catalogue
│   │   │   │   │   ├── components/
│   │   │   │   │   │   ├── CustomRoomAutoLaunchDialog.kt # 48-slot custom room grid & 1-tap launcher
│   │   │   │   │   │   ├── ScorecardDialog.kt       # Automated Gemini OCR scorecard reader
│   │   │   │   │   │   ├── MockUpiPaymentGateway.kt # Clean white 1-tap UPI payment simulator
│   │   │   │   │   │   ├── SlotBookingDialog.kt     # Slot picker and wallet check
│   │   │   │   │   │   ├── DocumentVerificationDialog.kt # Aadhaar/PAN/Voter KYC
│   │   │   │   │   │   ├── NextMatchCountdownCard.kt# Live tournament ticker
│   │   │   │   │   │   └── AdminBatchScheduleDialog.kt # Multi-room batch creator with custom timers
│   │   │   │   │   ├── theme/                       # Clean White, Gold/Amber & Red design system
│   │   │   │   │   └── viewmodel/EsportsViewModel.kt# Central state management
│   │   │   │   ├── data/
│   │   │   │   │   ├── db/AppDatabase.kt            # Room SQLite Database
│   │   │   │   │   ├── model/EsportsModels.kt       # Match, Registration, Transaction models
│   │   │   │   │   └── repository/EsportsRepository.kt
│   │   │   │   └── util/GameLauncherUtil.kt         # Free Fire / BGMI deep-linking & haptics
│   │   │   ├── res/                                 # Drawables, Adaptive App Icons, Strings
│   │   │   └── AndroidManifest.xml                  # Permissions, Activities
│   │   └── test/                                    # Unit tests & Robolectric test suite
│   └── build.gradle.kts                             # Kotlin Compose, Room, Coil, Coroutines
├── gradle/libs.versions.toml                        # Dependency version catalog
├── build.gradle.kts
└── settings.gradle.kts
```

---

## 🚀 Android Studio में रन करने का तरीका:
1. ZIP फाइल डाउनलोड करके अनज़िप करें।
2. Android Studio खोलें और `File -> Open` करके अनज़िप किया गया फोल्डर खोलें।
3. Gradle Sync अपने आप पूरा हो जाएगा।
4. `Run` (हरा प्ले बटन ▶) दबाएं और ऐप लाइव चलने लगेगा।
