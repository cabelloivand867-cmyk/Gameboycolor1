# Pocket Color (Game Boy / Game Boy Color emulator for Android)

A small Android app that wraps the emulator page in a WebView. No internet needed.
You load your own `.gb` / `.gbc` ROM files; none are included.

## Easiest: build the APK online with GitHub (no Android Studio)
1. Create a free account at github.com and make a new repository.
2. Upload everything in this folder (keep the folder structure, including `.github/workflows`).
3. Open the repository's **Actions** tab. The "Build APK" workflow runs on its own (or press Run workflow).
4. When it finishes (about 3-5 minutes), open the run and download `PocketColor-apk` at the bottom.
5. Unzip it, copy `app-debug.apk` to your phone, open it, and allow "install unknown apps" when asked.

## Or build with Android Studio
Open this folder in Android Studio, let it sync, then Build > Build APK(s).
Output: `app/build/outputs/apk/debug/app-debug.apk`.

## Notes
- Requires Android 8.0 or newer. Portrait only.
- Battery saves live in the app's own storage; clearing app data erases them.
- No sound yet. The emulator code is in `app/src/main/assets/index.html`.
