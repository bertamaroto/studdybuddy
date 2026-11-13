Study Buddy - Android WebView app
=================================

1. Install Android Studio (Hedgehog or newer): https://developer.android.com/studio
2. File > Open... and choose this StudyBuddy folder. Wait for Gradle sync to finish.
   (Android Studio downloads Gradle and the Android SDK 34 if it asks.)
3. Check the link in app/src/main/java/com/studybuddy/app/MainActivity.java
   (START_URL) points at your Study Buddy page.
4. Build > Build Bundle(s) / APK(s) > Build APK(s).
   The file appears in app/build/outputs/apk/debug/app-debug.apk
5. Copy it to the phone and install it (allow "install unknown apps" if asked),
   or run it directly on a connected phone / emulator with the green Run button.

Notes
- The app only shows the website inside a WebView. It needs internet.
- The page runs on claude.ai, so people must be signed in to Claude and have
  access to the page. Google sign-in often does not work inside WebViews;
  email sign-in is more reliable.
- Chats are saved inside the app's own storage on that phone.
- This project was written without being able to compile it, so if Android Studio
  reports a version warning, accept its suggested upgrade.
