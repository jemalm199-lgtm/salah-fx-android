SALAH FX — Android Studio project (v2.3.0)

WHAT THIS IS
This is an Android Studio source project that wraps the existing SALAH FX
web app in an Android WebView shell. It is NOT a compiled or signed APK yet.

BUILD AN APK
1. On a computer, install Android Studio (stable version) and Android SDK 35.
2. Extract this ZIP.
3. In Android Studio choose Open, then select the extracted SALAH_FX_Android_Project folder.
4. Allow Gradle sync and install any SDK components Android Studio requests.
5. Choose Build > Build Bundle(s) / APK(s) > Build APK(s).
6. Android Studio will show the APK location, normally:
   app/build/outputs/apk/debug/app-debug.apk
7. Copy that APK to your Android phone, tap it, and allow installation
   from that source if Android asks.

IMPORTANT LIMITATIONS
- This environment does not have the Android SDK or Gradle installed, so
  it cannot compile or sign an APK here. This ZIP is the source project.
- The Gemini backend is not deployed. The AI chat's /api/chat endpoint
  will not work in this local-file build until the app is configured to
  reach a deployed HTTPS backend. Never put a Gemini API key in the APK.
- This app does not connect to MT5, execute trades, stream live prices,
  or access broker accounts. Trading functions remain educational/manual.
- For a production release, use a proper launcher icon set, signing key
  stored securely, privacy policy, network/API hardening, and device tests.

PACKAGE
Application ID: com.salahfx.app
Version: 2.3.0
Minimum Android: 6.0 (API 23)
Target SDK: 35
