GLOBAL TRUCK SIMULATOR — ANDROID CLOUD BUILD KIT
================================================

Target:
- Android 10+ (minSdkVersion 29)
- ARM64-capable Android devices (Gradle's standard debug build may also include other ABIs)
- Landscape orientation
- Capacitor Android wrapper around the current Three.js browser prototype

IMPORTANT:
This ZIP is a SOURCE PROJECT + CLOUD BUILD WORKFLOW. It is NOT an APK.
The APK is produced by GitHub Actions after you upload this project to a GitHub repository
and run the workflow. No Windows PC is required; the upload and workflow can be managed
from your Android phone's browser, although a GitHub account is required.

PHONE-ONLY BUILD STEPS:
1. Sign in to GitHub or create an account at https://github.com.
2. Create a new repository named global-truck-simulator-android.
3. Upload the CONTENTS of this ZIP into the repository (not the ZIP itself).
   Make sure package.json, capacitor.config.json, www/, and .github/ are at repository root.
4. Open the repository's Actions tab.
5. Select "Build Android APK" and press "Run workflow".
   If Actions are disabled, enable them in the repository's Actions settings.
6. Wait for the workflow to finish successfully.
7. Open the completed workflow run, scroll to Artifacts, and download
   Global-Truck-Simulator-Android-APK.
8. Extract the downloaded artifact ZIP on your phone, tap app-debug.apk,
   and allow installation from that source if Android asks.

PACKAGE:
Application ID: com.globaltrucks.simulator
App name: Global Truck Simulator
Minimum SDK: 29 (Android 10)
Build type: Debug APK (installable for testing; not Play Store release-signed).

LIMITATIONS OF THIS PROTOTYPE:
- This is a wrapper around the existing Three.js prototype, not a native Unity-grade simulator.
- Three.js is loaded from unpkg CDN, so the first launch and gameplay require internet.
- The current scene uses procedural placeholder truck/road/traffic geometry.
- Career, multiple countries, real cargo economy, refuelling, advanced AI traffic,
  realistic trailer articulation and full simulation physics are not yet implemented.
- A release APK suitable for public distribution should be signed with a private keystore
  and thoroughly tested on physical devices.

Troubleshooting:
- If the GitHub Actions workflow fails, open the failed job and download/copy the error log.
- Do not share passwords, access tokens, signing keys, or private keystores in chat.
