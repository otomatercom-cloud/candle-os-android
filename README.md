# Candle OS Android app

Opens https://os.candleelectric.in inside an Android app (WebView). Everything stays on the server:
updates to Candle OS appear in the app immediately, no new APK needed.
Permissions: camera (photo + video), microphone (video sound), location (GPS), photos/videos, internet.

## Get the APK (no Android Studio)
1. Create a PRIVATE GitHub repo, upload everything in this folder (keep the .github folder).
2. GitHub -> Actions -> "Build Candle OS APK" -> Run workflow.
3. After ~5-8 minutes open the run -> Artifacts -> candle-os-apk -> download, unzip -> app-debug.apk.
4. Copy the APK to the phone, open it, allow "Install unknown apps", install.

## Or with Android Studio
npm install && npx cap sync android && npx cap open android, then Build -> Build APK(s).

## Change the server address
Edit capacitor.config.json -> server.url, then npx cap sync android and rebuild.
