# Mr. Parking – Android project

This folder wraps the Mr. Parking game (app/src/main/assets/index.html) in a tiny Android app.

## Easiest: build the APK online with GitHub (no installs)
1. Create a free GitHub account and a new empty repository.
2. Upload the contents of this folder (keep the `.github` folder).
3. Open the repository's **Actions** tab, choose **Build APK**, click **Run workflow**.
4. When it finishes (~3-5 min), open the run and download the **MrParking-apk** artifact (a zip containing `app-debug.apk`).
5. Copy the APK to your phone and open it. Android will ask to allow "Install unknown apps" for your browser/file manager – allow it once.

## Or: build with Android Studio
Open this folder in Android Studio, let it sync, then **Build > Build APK(s)**.
The APK appears in `app/build/outputs/apk/debug/`.

## Notes
- The APK is debug-signed: fine for installing on your own phone. Publishing to Google Play needs a release-signed build (AAB) instead.
- The game saves progress inside the app. Uninstalling removes the saves.
- The game loads one font from Google Fonts, so the first launch looks best online; it still runs offline.
- Remember the temporary **Dev Mode** button is still on the main menu.
