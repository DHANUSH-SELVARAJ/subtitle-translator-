# Tamil Subtitles (Android)

Floating English→Tamil vocabulary helper for any video app. Uses screen capture (with your
permission), on-device OCR (Google ML Kit) and the same word-filtering logic as the Windows version.

## Get the APK without Android Studio (GitHub builds it)
1. Create a free GitHub account and a new repository (e.g. `tamil-subtitles`).
2. Upload ALL files and folders of this project (keep the folder structure, including `.github/`).
3. Open the repo → **Actions** → **Build APK** → wait ~5 minutes (or press **Run workflow**).
4. Open the finished run → **Artifacts** → download `TamilSubtitles-apk` (a zip containing `app-debug.apk`).
5. On the phone: unzip, tap the APK, allow "Install unknown apps" for your browser/file manager.

Or with Android Studio: open this folder → Build → Build APK(s).

## Use
1. Open the app → **Allow "Display over other apps"**.
2. Move the two sliders so the band covers where subtitles appear.
3. **Start translation** → accept the screen-capture prompt → open your video.
4. New words appear in the floating window. **Mark Known** hides a word for good; **History** opens the saved list.

## Limits
- Words come from a ~70-entry offline SAMPLE dictionary; others are skipped (listed in the app).
- Apps that block capture (DRM / secure windows) give black frames; this is not bypassed.
- Keep the floating window outside the subtitle band, or it may be read by OCR.
- Android asks for screen-capture permission each time you start.
- Source written without being compiled in the build sandbox (no Android SDK): expect to fix small build errors.
