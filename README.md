# HomeCare Android APK project

This is a free, open-source Android WebView wrapper for the HomeCare maintenance tracker prototype.

## Build a free installable APK using GitHub Actions

1. Create a free GitHub account if you don't already have one.
2. Create a new repository named `HomeCare` (a public repository avoids using private-repository Actions minutes).
3. Upload the contents of this folder to the repository root.
4. Open the repository's **Actions** tab and select **Build HomeCare APK**.
5. Press **Run workflow**. Wait for the workflow to finish.
6. Open the completed run, scroll to **Artifacts**, and download `HomeCare-debug-apk`.
7. Extract the ZIP on your Android phone and tap `app-debug.apk`.
8. If Android asks, allow Chrome or Files to install unknown apps, then install HomeCare.

## Important prototype limitations

- This package embeds the current HomeCare HTML app in Android WebView. Its task data is stored locally in the app's WebView storage.
- This is a debug APK for personal testing, not a Play Store release.
- The current reminder code checks while the app is running/active. Android WebView does not provide reliable scheduled background notifications from the existing browser-notification code. Native Android scheduled notifications and reboot recovery still need to be implemented and tested before calling reminders dependable.
- The current language recognition is rule-based phrase matching, not a connected AI model.
- Export backups from HomeCare before uninstalling or clearing app data.

No paid developer account or Play Store listing is required for this personal debug APK.
