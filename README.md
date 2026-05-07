# Bud — Offline AI Companion

Bud is a mobile app that lets you run AI conversations directly on your device — no subscription, no account required. You download an AI model once, and it runs fully on your phone.

---

## Download

| Platform | File | Size |
|----------|------|------|
| Android  | [Bud-v1.0.1.apk](./Bud-v1.0.1.apk) | ~70 MB |
| iOS      | [Bud-v1.0.1.ipa](./Bud-v1.0.1.ipa) | ~13 MB |

---

## Install on Android

1. Download `Bud-v1.0.1.apk` to your Android device.
2. Open your file manager and tap the APK.
3. If prompted, go to **Settings → Install unknown apps** and allow your file manager or browser.
4. Tap **Install** and open the app.
5. On first launch, go to the **Models** tab and download an AI model (requires Wi-Fi, ~1–4 GB depending on the model).

> Tested on Android 7.0+ (API 24 and above). ARM64 devices only (all modern Android phones qualify).

---

## Install on iOS

iOS does not allow installing IPA files from outside the App Store without a workaround. Choose one:

### Option A — AltStore (free, no jailbreak)

1. Install [AltStore](https://altstore.io) on your Mac or PC.
2. Connect your iPhone via USB and trust the computer.
3. In AltStore on your computer, click **+** and select `Bud-v1.0.1.ipa`.
4. Sign in with your Apple ID when prompted (used only for local signing — no data is sent to us).
5. Open Bud on your iPhone.
6. Go to **Settings → General → VPN & Device Management** and trust the developer certificate.

### Option B — Sideloadly (free, no jailbreak)

1. Download [Sideloadly](https://sideloadly.io) on your Mac or PC.
2. Connect your iPhone, select `Bud-v1.0.1.ipa`, and click **Start**.
3. Enter your Apple ID when prompted.
4. Trust the certificate on your iPhone: **Settings → General → VPN & Device Management**.

### Option C — Register your UDID (contact us)

If you want a build signed directly for your device with no re-signing needed, send us your device UDID and we'll add it to the provisioning profile.

> **Re-signing note:** Free Apple IDs expire the sideload every 7 days; paid developer accounts last 1 year. You'll need to re-sideload when it expires.

---

## What Bud Does

- Runs open-source LLM models (Llama, Mistral, and compatible GGUF models) directly on your device using [llama.cpp](https://github.com/ggml-org/llama.cpp).
- No data leaves your device during inference — the model runs entirely on-device.
- You pick and download models from Hugging Face directly within the app.

---

## Honest Note on Cloud Sync for AI Agents

Bud has a **Buds** feature — a catalog of AI personas (custom system prompts with names and icons). This catalog is synced from a shared [Supabase](https://supabase.com) database.

Here is what that means honestly:

- **The Buds catalog is fetched from our Supabase project** on first launch and periodically in the background. This is a network request to our server.
- **Your conversations are never sent anywhere.** Chat history stays on your device.
- **Custom Buds you create** can be published to the shared catalog, making them visible to all users. This uploads the bud's name, description, system prompt, and icon to our Supabase database. There is no moderation in the current version — what you publish goes live immediately.
- **If you do not create or publish a Bud**, nothing from your device is uploaded.
- The Supabase project is `cvjjmfqgpnsshcekffmm` (hosted on Supabase's US infrastructure). We do not control Supabase's own data handling — see [Supabase's privacy policy](https://supabase.com/privacy) for details.
- There is no authentication. All catalog reads and writes use the anonymous Supabase key embedded in the app. This means anyone with the key could read the catalog — treat anything you publish as public.
- Delta sync runs in the background after launch to pull catalog updates. It makes a small HTTP request with a timestamp filter. No device identifiers are sent.

**Summary:** your AI conversations are private and local. The only cloud component is the shared Bud persona catalog, and only content you explicitly choose to publish is uploaded.

---

## Requirements

| | Android | iOS |
|---|---|---|
| Minimum OS | Android 7.0 (API 24) | iOS 16+ |
| Architecture | ARM64 | ARM64 |
| Storage needed | 500 MB app + model size (1–8 GB) | 500 MB app + model size |
| RAM recommended | 4 GB+ | 4 GB+ |

---

## Version

`v1.0.1` — May 2025
