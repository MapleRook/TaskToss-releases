# TaskToss Privacy Policy

**Last updated:** April 25, 2026
**Contact:** tasktoss@proton.me

TaskToss is a task management and reminder app built by Dalton Haglund. This policy explains what data the app collects, how it is used, who it is shared with, and your rights.

---

## 1. Information We Collect

### 1a. Data stored locally on your device

All of the following data is stored exclusively on your device and **never transmitted to any server** unless you explicitly initiate an action that requires it (such as AI capture parsing):

- **Tasks and notes** — titles, descriptions, due dates, priority, categories, completion status
- **Recurring reminder logs** — timestamps and optional star ratings for recurring tasks you log as completed
- **Event logs** — timestamps and types of actions you take in the app (completions, reschedules, etc.), used to power your on-device analytics
- **App settings and preferences** — notification preferences, display settings, reminder configuration

### 1b. Data transmitted to our server

When you use the **Free** or **Pro** AI capture feature, the following is sent to our processing server (`tasktoss-api.tasktoss.workers.dev`, hosted on Cloudflare Workers):

- **Your capture text** — forwarded to the Anthropic API (Claude) for parsing into structured tasks and notes. Your text is not stored on our server and is not retained after processing.
- **Device identifier** — a randomly generated ID stored on your device, used solely to enforce the free-tier daily usage limit. This ID has no connection to your identity, device hardware, or any other personal information.
- **Time context** — your local time, timezone, and day of week, used to correctly interpret time references in your captures (e.g., "tomorrow", "after work").

When you use the **Pro** plan:

- **Your email address** — sent to our server to verify your subscription status against Stripe. This is checked in real time and cached for up to 24 hours for performance. It is not used for any other purpose.

### 1c. Data in Bring Your Own Key (BYOK) mode

If you use the BYOK option, your capture text is sent **directly from your device to the Anthropic API** using your own API key. It does not pass through our server at any point.

### 1d. Crash reports

TaskToss uses Sentry for crash reporting. When the app crashes, a report is automatically sent containing:

- Device type, operating system version, and app version
- Stack trace (technical error details)

Crash reports **never** contain your task content, notes, or any personal information. The Sentry SDK is configured to strip identifying information before transmission.

### 1e. Data we do NOT collect

- We do not collect your name, phone number, or physical address
- We do not collect your location or GPS data
- We do not access your contacts, camera, microphone, or files
- We do not use advertising SDKs or tracking pixels
- We do not create user profiles for advertising purposes
- We do not collect device hardware identifiers (IMEI, MAC address, etc.)

---

## 2. How We Use Your Information

| Data | Purpose | Legal basis |
|------|---------|-------------|
| Capture text | Parse into structured tasks/notes via AI | Contractual necessity (providing the service) |
| Device identifier | Enforce free-tier daily usage limit | Legitimate interest (preventing abuse) |
| Email (Pro) | Verify subscription status | Contractual necessity |
| Time context | Interpret time references in captures | Contractual necessity |
| Crash reports | Identify and fix bugs | Legitimate interest (improving the service) |
| Analytics (opt-in) | Understand feature usage patterns | Consent |

---

## 3. How We Share Your Information

**We do not sell your personal information.** We never have and never will.

We share data only with the following service providers, solely to operate the app:

| Provider | Purpose | Data shared | Their privacy policy |
|----------|---------|-------------|---------------------|
| **Anthropic** | AI text parsing | Capture text (transient, not stored) | [anthropic.com/privacy](https://www.anthropic.com/privacy) |
| **Stripe** | Payment processing (Pro plan) | Email, payment details (handled by Stripe) | [stripe.com/privacy](https://stripe.com/privacy) |
| **Cloudflare** | Server infrastructure | Capture text passes through (not stored) | [cloudflare.com/privacypolicy](https://www.cloudflare.com/privacypolicy/) |
| **Sentry** | Crash reporting | Device info, stack traces (no personal data) | [sentry.io/privacy](https://sentry.io/privacy/) |

We do not share data with any other third parties, advertisers, or data brokers.

---

## 4. Data Retention and Deletion

- **On-device data:** Retained until you delete it or uninstall the app. You have full control.
- **Server-side:** We do not store your capture text or personal data on our servers. Rate-limit counters (device ID + daily count) are automatically deleted after 48 hours. Pro subscription verification caches expire within 24 hours.
- **Crash reports:** Retained in Sentry for 90 days, then automatically deleted.
- **Stripe:** Payment data is retained by Stripe according to their retention policy and legal obligations.

**To delete all your data:** Uninstall the app. All local data is permanently removed. If you had a Pro subscription, you can request deletion of your Stripe customer record by contacting tasktoss@proton.me.

---

## 5. Security

- All data transmitted between the app and our server uses HTTPS/TLS encryption
- All data transmitted to third-party services (Anthropic, Stripe, Sentry) uses HTTPS/TLS encryption
- On-device data is protected by your device's built-in encryption and lock screen
- Our server (Cloudflare Worker) is stateless — it does not store any user data at rest
- API keys (BYOK mode) are stored locally on your device and never transmitted to our server

---

## 6. Your Rights

### All users

- **Access and export:** Export all your data at any time via Settings > Backup & Restore
- **Deletion:** Uninstall the app to delete all local data
- **Opt-out of analytics:** Analytics are off by default. If enabled, disable them at any time in Settings
- **Choice of plan:** Choose Free, Pro, or BYOK to control how your data is processed

### European Economic Area (EEA) and UK residents (GDPR)

You have the right to access, rectify, erase, restrict processing of, and port your personal data. You may also object to processing based on legitimate interest. Since your data is stored locally and we act as a minimal processor for transient AI requests, most of these rights are satisfied by the app's built-in controls. For any requests we need to handle server-side, contact tasktoss@proton.me.

### California residents (CCPA/CPRA)

You have the right to know what personal information we collect, to request its deletion, and to opt out of its sale. **We do not sell personal information.** The categories of personal information we process are described in Section 1 above. To exercise your rights, contact tasktoss@proton.me.

---

## 7. International Data Transfers

Our processing server is hosted on Cloudflare's global network. Anthropic (AI processing) and Stripe (payments) are based in the United States. If you are located outside the United States, your capture text and email (Pro only) may be transferred to and processed in the United States. These transfers are protected by HTTPS encryption and the service providers' data protection agreements.

---

## 8. Children's Privacy

TaskToss is not directed at children under 13. We do not knowingly collect personal information from children under 13. If you believe a child has provided us with personal information, contact us at tasktoss@proton.me and we will take steps to delete it.

---

## 9. Optional Analytics

TaskToss includes an anonymous analytics feature that is **disabled by default**. If you choose to enable it in Settings:

- Only aggregate usage patterns are collected (which features are used, completion rates, reminder effectiveness)
- No task content, note content, or personal information is ever included
- No advertising identifiers or cross-app tracking is used
- You can disable it at any time in Settings with immediate effect

---

## 10. Changes to This Policy

We may update this policy from time to time. The updated version will be posted at the same URL with a revised "Last updated" date. Material changes will be communicated through the app. Continued use of the app after changes constitutes acceptance of the updated policy.

---

## 11. Contact

For privacy questions, data requests, or concerns:

**Email:** tasktoss@proton.me

We aim to respond to all requests within 30 days.
