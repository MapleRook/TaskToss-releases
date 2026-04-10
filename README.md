# TaskToss

ADHD-friendly task capture with escalating reminders. Toss everything from your head into the inbox — AI sorts it into tasks, notes, and reminders.

## Features

- **AI-powered capture** — type naturally ("dentist thursday at 2, pick up meds tomorrow morning, remember to call mom") and AI parses it into structured tasks with due dates, priorities, and reminder styles
- **Escalating reminders** — nudge, nag, or nuclear. Reminders auto-escalate after repeated reschedules. Nuclear = full-screen takeover with alarm
- **Medication tracking** — log when you take meds, see cognitive zone overlays (green/yellow/red) on your calendar and task list
- **Calendar day/week/month views** — timeline with transition blocks, free time, and medication zone shading
- **Shopping lists** — auto-categorized by store from natural language input
- **Knowledge base** — AI-formatted reference cards from messy notes
- **Gamification** — XP, levels, and achievements for completing tasks
- **Quick capture widget** — home screen widget for instant thought capture
- **Backup/restore** — full JSON export/import to Downloads

## Install

1. Download the latest APK from [Releases](https://github.com/MapleRook/TaskToss-releases/releases)
2. On your Android device, enable "Install unknown apps" for your file manager or browser
3. Open the APK and install
4. Walk through the 7-step setup (permissions + plan selection)

## Plans

| Plan | Price | What you get |
|------|-------|-------------|
| **Free** | $0 | 10 AI captures/day. No setup required. |
| **Bring Your Own Key** | Pay Anthropic directly | Unlimited captures + all AI features. Paste your own [Anthropic API key](https://console.anthropic.com/). Typically pennies/day. |
| **Pro** | $4.99/mo | Coming soon. Unlimited, no key juggling. |

## Requirements

- Android 8.0+ (API 26)
- ~3 MB install size

## Privacy

- All task data stored on-device only
- API key (BYOK mode) stored in Android EncryptedSharedPreferences, transmitted only to api.anthropic.com
- Free tier requests routed through our server for AI parsing — no task content is stored server-side
- Optional anonymous analytics (off by default, must be explicitly opted in)
- No ads. No tracking. No selling data. Ever.
