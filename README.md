# Bud: Offline AI

Private, on-device AI for iOS and Android. No cloud. No subscriptions. Nothing leaves your phone.

## Download

| Platform | File |
|----------|------|
| Android (APK) | [Bud-v1.0.6.apk](./Bud-v1.0.6.apk) |
| iOS (IPA) | [Bud-v1.0.6.ipa](./Bud-v1.0.6.ipa) |

**Android:** Tap the APK, enable "Install unknown apps" if prompted.  
**iOS:** Sideload with [Sideloadly](https://sideloadly.io) or [AltStore](https://altstore.io). After install: Settings > General > VPN & Device Management > Trust.

---

## What it does

- Fully offline inference and no internet after setup
- 20+ AI personas across productivity, code, education, healthcare, lifestyle
- Browse and download models from Hugging Face directly in-app
- Metal GPU acceleration on iOS, voice mode, document scanning
- The Bud persona has live device access: calendar, contacts, reminders, web search
- Chat history stored locally, dark/light mode

---

## First Launch

Go to the **Models** tab, pick a model, and download it over Wi-Fi. Recommended starting point: **Llama 3.2 1B** (~800 MB, runs on any device).

---

## Privacy

Conversations stay on-device. The only network request is syncing the Bud catalog on launch. No login, no analytics, no tracking.

---

## Version History

| Version | Notes |
|---------|-------|
| v1.0.6 | Camera/gallery attachments now reach the model (OCR at pick-time), chat input no longer half-opaque over glass footer, voice mode recovers from stuck-listening state, long-context survival via tiered conversation compaction (extractive + LLM rolling summary), CPU thread auto-tune, post-load config logging, model health check |
| v1.0.5 | Attachment stability: scan permission fix, image OOM crash fix, memory-efficient OCR, Flutter image cache constraints, low memory toast |
| v1.0.4 | Freewill AI personas, conditional glass footer bar, full-height filter drawer, curated model icons in chat history, share export icon |
| v1.0.3 | Capability icons on model cards, custom toast notifications, inference chip with info drawer, scan fix, settings auto-sync after model load, low-end device memory fixes |
| v1.0.2 | Supabase delta sync, Create Bud screen |
| v1.0.1 | Initial release |
