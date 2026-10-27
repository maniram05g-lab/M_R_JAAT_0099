# Study AI Hindi — Android प्रोजेक्ट

यह Chrome/HTML पेज नहीं, Android Studio में APK बनाने के लिए native Android प्रोजेक्ट है।

## इसमें क्या है
- ऐप खुलने पर 3 सेकंड splash screen
- फोटो के बिना ऐप; Splash screen पर “MR JAT” बड़ा दिखाई देता है
- जवाब चुनने पर “MR JAT” का फुल-स्क्रीन पॉप-अप लगभग 1.25 सेकंड दिखता है, फिर उसी सवाल पर वापस आता है
- 50 अलग-अलग MCQ: Maths, Reasoning, GK, Science, Hindi, English
- 30 मिनट का टाइमर
- चार विकल्प, अगला/पिछला, सवाल सूची
- सही उत्तर +1, गलत उत्तर −0.33, छोड़े गए सवाल पर 0
- रिजल्ट, accuracy और टेस्ट हिस्ट्री
- पुराने टेस्ट के जवाब और सॉल्यूशन फिर से देखना
- डेटा फोन में लोकली सेव होता है; इस शुरुआती संस्करण में लॉगिन/क्लाउड सिंक नहीं है

## APK कैसे बनाएं
1. कंप्यूटर पर Android Studio इंस्टॉल करें: https://developer.android.com/studio
2. ZIP extract करें। Android Studio में `StudyAIHindi` फ़ोल्डर खोलें।
3. Gradle sync पूरा होने दें। SDK 35 डाउनलोड करने को कहे तो स्वीकार करें।
4. `Build > Build Bundle(s) / APK(s) > Build APK(s)` चुनें।
5. APK सामान्यतः `app/build/outputs/apk/debug/app-debug.apk` में मिलेगा।
6. APK को फोन में भेजकर इंस्टॉल करें। फोन में पूछे तो केवल इस फ़ाइल मैनेजर/ब्राउज़र के लिए “Install unknown apps” अनुमति दें। अनजान वेबसाइटों से APK न लें।

## जरूरी सच
इस वातावरण में Android SDK/Gradle build tool उपलब्ध नहीं था, इसलिए यहाँ तैयार और टेस्ट किया हुआ APK binary नहीं बनाया गया। यह Android source project है जिसे Android Studio से build करना होगा। इसे रिलीज़ करने से पहले सभी प्रश्नों/समाधानों का पुनरीक्षण और वास्तविक डिवाइस पर परीक्षण करें।
