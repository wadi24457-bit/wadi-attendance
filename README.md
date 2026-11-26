# wadi-attendance (حضور وانصراف)

Employee check-in/check-out app (Arabic, RTL). Pay month runs from the 26th to the 25th. Data syncs through Supabase (publishable key in the source, protected by row-level security).

- `site/app.html` is the live app (https://wadi-attendance.surge.sh/app.html). `site/index.html` is the landing stub.
- `dist/attendance.apk` is the Android build (com.wadi.attendance v1.1). It is a WebView wrapper around the app.
- `android/` holds what could be recovered from the APK: the bundled offline copy of the page, the launcher icons and the manifest dump. The original Java sources and signing key were not kept, so the APK cannot be rebuilt from this repo; to ship an update, edit `site/app.html` and redeploy it (the app loads it from the web).

This repo was mirrored from the deployed files. No keystore or secrets are included.
