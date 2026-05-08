# Bud: Offline AI Companion

Chat with open-source AI models on your phone. No account, no subscription. Models run on-device.

## Download

| Platform | File | Size |
|----------|------|------|
| Android | [Bud-v1.0.2.apk](./Bud-v1.0.2.apk) | ~70 MB |
| iOS | [Bud-v1.0.3.ipa](./Bud-v1.0.3.ipa) | ~13 MB |

---

## Install on Android

1. Download **Bud-v1.0.2.apk** to your Android phone.
2. Tap the downloaded file in your browser or Files app.
3. If prompted, tap **Settings** and enable **Install unknown apps**, then go back and tap **Install**.
4. Open **Bud** from your home screen.

Requires Android 7.0+, ARM64 (all phones from 2017 onward).

---

## Install on iOS (iPhone / iPad)

iOS requires a free tool on your computer to sideload the IPA. **Sideloadly** is the easiest.

### Option 1: Sideloadly (Recommended)

1. Download **[Sideloadly](https://sideloadly.io)** on your Mac or Windows PC.
2. Connect your iPhone with a USB cable.
3. Drag **Bud-v1.0.3.ipa** into the Sideloadly window.
4. Enter your Apple ID when prompted (used only for local signing).
5. Click **Start**. The app installs in about a minute.
6. On iPhone: **Settings > General > VPN & Device Management** > tap your Apple ID > **Trust**.
7. Open **Bud**.

Free Apple ID: repeat every 7 days (one click in Sideloadly). Paid developer account: valid 1 year.

### Option 2: AltStore

1. Download **[AltStore](https://altstore.io)** and install AltServer on your Mac or PC.
2. Connect your iPhone via USB, open AltServer > Install AltStore > select your device.
3. Open AltStore on iPhone, tap **+**, and select **Bud-v1.0.3.ipa**.
4. Trust the certificate: **Settings > General > VPN & Device Management**.

Same 7-day refresh for free Apple IDs.

---

## First Launch

Accept the Terms of Use, then go to the **Models** tab to download a GGUF model from Hugging Face. Requires Wi-Fi. Model sizes range from 500 MB to several GB.

---

## Privacy

- Conversations stay on your device and are never sent anywhere.
- The Buds catalog (AI personas) is synced from a shared database on launch. That is the only network request the app makes by default.
- Publishing a Bud uploads its name, icon, description, and system prompt to the shared database. It is immediately visible to all users. No moderation. Treat it as fully public.
- No login. No analytics. No tracking.

---

## Version History

| Version | Notes |
|---------|-------|
| v1.0.3 | Report buds, Terms of Use on first launch, manual Publish to Community, Offline AI branding, maintenance mode |
| v1.0.2 | Supabase delta sync, Create Bud screen, AppBar create button |
| v1.0.1 | Initial release |
