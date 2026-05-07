# Bud: Offline AI Companion

Chat with open-source AI models on your phone. No account, no subscription. Models run on-device.

## Download

| Platform | File | Size |
|----------|------|------|
| Android | [Bud-v1.0.2.apk](./Bud-v1.0.2.apk) | ~70 MB |
| iOS | [Bud-v1.0.2.ipa](./Bud-v1.0.2.ipa) | ~13 MB |

## Install on Android

1. Download `Bud-v1.0.1.apk` to your device.
2. Tap the file in your file manager.
3. If prompted, enable **Install unknown apps** for your file manager or browser.
4. Tap **Install**.

Requires Android 7.0+ (API 24), ARM64 only. All modern Android phones qualify.

## Install on iOS

iOS requires sideloading. Use one of these free tools:

**AltStore** ([altstore.io](https://altstore.io))
1. Install AltStore on your Mac or PC.
2. Connect your iPhone via USB.
3. In AltStore, tap **+** and select `Bud-v1.0.1.ipa`.
4. Sign in with your Apple ID (used for local signing only).
5. On your iPhone, go to **Settings > General > VPN & Device Management** and trust the certificate.

**Sideloadly** ([sideloadly.io](https://sideloadly.io))
1. Install Sideloadly on your Mac or PC.
2. Connect your iPhone, select the IPA, and click **Start**.
3. Enter your Apple ID when prompted.
4. Trust the certificate on your iPhone under **Settings > General > VPN & Device Management**.

Free Apple IDs need re-sideloading every 7 days. Paid developer accounts last 1 year.


## First Launch

Go to the **Models** tab and download a GGUF model from Hugging Face. Requires Wi-Fi and storage space depending on the model you choose.

## Cloud Sync (Buds Catalog)

Bud includes a **Buds** feature: a shared catalog of AI personas with custom names, icons, and system prompts. This is the only part of the app that touches a server.

- The catalog is fetched from a shared Supabase database on launch and synced periodically in the background.
- Your conversations stay on your device and are never sent anywhere.
- If you create and publish a Bud, its name, description, system prompt, and icon are uploaded to the shared database and are visible to all users immediately. There is no moderation.
- If you never publish a Bud, nothing from your device is uploaded.
- There is no login. The app uses an anonymous Supabase key. Treat anything you publish as fully public.

## Version

`v1.0.2` released May 2026
