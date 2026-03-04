# Privacy Policy

Effective date: March 4, 2026

Faith Flow is designed to be privacy-first.

## Summary

- We do not require email addresses, names, or social accounts to use the app.
- We do not sell your personal data.
- Your personal devotional content (notes, journal entries, bookmarks, highlights, and related progress data) is stored locally on your device.
- Sensitive local data is protected with device-backed security and encryption at rest.
- Biometric data (Face ID/Fingerprint) is handled by your device OS and never sent to Faith Flow.
- Certain features (Prayer Wall, push notifications, AI devotionals) require limited data to be sent to servers as described below.

## Data Stored Locally on Your Device

Faith Flow stores the following categories locally on your device and does **not** transmit them to any server:

- Bible reading preferences and app settings
- Bookmarks, highlights, notes, and journal entries
- Streaks, devotional progress, and challenge progress
- Notification preferences and reminder times
- Voice command settings

This data is encrypted at rest and unlocked using device authentication (biometric or device passcode/PIN/pattern fallback).

## Data Sent to Servers

Some features require limited data to be processed on external servers:

### Prayer Wall (Firebase / Google Cloud)
When you submit a prayer request, the following is sent to and stored in Google Firebase (Firestore):
- Your prayer text (after content moderation)
- A server-generated anonymous display name (e.g., "Believer #42")
- Your anonymous user ID (a random identifier — not your name or email)
- The prayer category you selected
- A server timestamp

Prayer requests are publicly visible to other app users. **Do not include personally identifiable information in prayer requests.**

### Anonymous Authentication (Firebase)
Faith Flow creates an anonymous Firebase account using a random device-generated UUID. This does not require your name, email, or any personal information. The anonymous user ID is used to:
- Link your prayer submissions to a consistent display name
- Enforce rate limits on prayer submissions and AI requests
- Enable device recovery via recovery keys

A cryptographic hash of your device UUID is stored in Firestore to support device recovery. No plaintext device identifiers are stored on our servers.

### Push Notifications (Firebase Cloud Messaging)
If you opt in to push notifications, a Firebase Cloud Messaging (FCM) token is stored in Firestore to deliver notifications to your device (e.g., when someone prays for your request). You can opt out at any time by revoking notification permission in your device settings.

### AI-Powered Features (Third-Party AI Services)
When you use AI features (e.g., devotional generation, Bible Q&A), your prompt text is sent through our server (Cloudflare Workers) to third-party AI providers such as OpenRouter, Groq, or Hugging Face. **We do not store your prompts or AI responses on our servers.** These providers process your text according to their own privacy policies:
- [OpenRouter Privacy Policy](https://openrouter.ai/privacy)
- [Groq Privacy Policy](https://groq.com/privacy-policy/)
- [Hugging Face Privacy Policy](https://huggingface.co/privacy)

### App Integrity (Firebase App Check / reCAPTCHA)
To protect the app from abuse, Faith Flow uses Firebase App Check with reCAPTCHA Enterprise (web) and Play Integrity (Android). These services may collect device signals such as IP address and app attestation data. This data is processed by Google according to the [Google Privacy Policy](https://policies.google.com/privacy) and [reCAPTCHA Terms](https://policies.google.com/terms).

## Cloud Backups (Apple / Google)

If you enable device backup services (such as iCloud Backup or Google account/device backup), your locally stored app data may be included in those backups according to your Apple/Google settings.

- Those backups are managed by Apple/Google under their own terms and privacy policies.
- Faith Flow does not operate those backup services.
- You control backup behavior in your device/cloud account settings.

## Permissions

Faith Flow requests only the permissions needed for app features:

- **Biometric/device credential authentication** — for app security. Biometric data (Face ID/fingerprint) is handled entirely by your device OS and never leaves your device.
- **Notifications** — for prayer reminders and verse-of-the-day alerts. You choose when and how often.
- **Microphone (RECORD_AUDIO)** — for optional voice commands that let you navigate the app hands-free (e.g., "next chapter", "read aloud", "stop"). Audio is processed in real time using your device's built-in speech recognition service (e.g., Google Speech Services on Android). **Faith Flow does not record, store, or transmit your audio.** Speech recognition results are used only to match commands within the app and are discarded immediately. Your device's speech service may process audio according to its own privacy policy (see [Google Privacy Policy](https://policies.google.com/privacy)).
- **Internet / Network State** — to load Bible translations, sync prayer wall data, and deliver push notifications.
- **Storage** — for offline Bible data caching (Android 9 and below only).

You can deny or revoke any permission at any time in your device settings. Voice commands are disabled by default and only activate when you choose to enable them.

## Data Sharing

Faith Flow does not share your data with third parties for advertising or profiling. Data is shared with third parties only as described above (Firebase/Google for authentication, storage, and notifications; AI providers for AI features) and only to the extent necessary to deliver the requested feature.

## Data Retention and Deletion

- **Local data:** remains on your device unless you remove it, uninstall the app, or clear app storage.
- **Prayer wall posts:** remain in Firestore until removed by moderation or service shutdown.
- **Anonymous accounts and FCM tokens:** retained in Firebase until the account is deleted or becomes inactive per Firebase's retention policies.
- **AI prompts:** not retained by Faith Flow. Third-party AI providers may retain data per their own policies.
- **Cloud backups:** follow your Apple/Google backup settings and retention rules.

To request deletion of your server-side data, contact us at the email below.

## Children

Faith Flow is not directed to children under 13.

## Changes to This Policy

We may update this policy from time to time. The updated version will include a new effective date.

## Contact

For privacy questions or data deletion requests, contact: wesleykthedev@gmail.com


Faith Flow — Data Deletion Request

Faith Flow does not require user accounts. All personal data (notes, bookmarks, highlights, journal entries) is stored locally on your device and can be deleted by clearing app data or uninstalling.

To request deletion of server-side data (prayer wall posts, anonymous identifiers, push notification tokens), email wesleykthedev@gmail.com.

Data deleted: prayer submissions, anonymous user ID, FCM token, rate limit records.
Typical processing time: within 30 days.