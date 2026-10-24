# Deepak's Rent Book (Android app)

A native Android app (Kotlin) that holds the rent book inside it. It works offline, keeps its records on the phone, and needs Android 10 or newer.

The rent book itself is `app/src/main/assets/index.html`. The Kotlin code in `MainActivity.kt` only shows that page, opens the dialer for Call buttons, saves backup files to the Downloads folder, and lets Restore pick a backup file.

## Get the APK, option 1: Android Studio (on a computer)

1. Install Android Studio (free, developer.android.com/studio).
2. Unzip this folder. In Android Studio choose File > Open and pick the `DeepakRentBook` folder. Wait for the first sync to finish.
3. Choose Build > Build Bundle(s) / APK(s) > Build APK(s).
4. Click "locate" in the pop-up. The file is `app-debug.apk`.
5. Send `app-debug.apk` to the phone (WhatsApp, Drive or a cable), open it, and allow "Install unknown apps" when Android asks.

To test first, connect the phone with USB debugging on and press the green Run button instead.

## Get the APK, option 2: GitHub (no Android Studio)

1. Create a free GitHub account and a new repository.
2. Upload every file and folder from this project, including the hidden `.github` folder.
3. Open the Actions tab, choose "Build APK", press Run workflow.
4. When it finishes (a few minutes), open the run and download the `rent-book-apk` file. It contains `app-debug.apk`.

## Notes

- The first build downloads the Android build tools, so it needs internet.
- The debug APK is fine for personal use. For the Play Store you would need a release build signed with your own key.
- Records live inside the app. Uninstalling the app deletes them, so use Download backup in the app first.
