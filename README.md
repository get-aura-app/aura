# Aura — a local-first AI assistant for Android

Aura is an AI assistant that runs **entirely on your phone**. The language
model (Google's Gemma 4 E2B, via LiteRT-LM) is downloaded once and then
runs on-device: no account, no cloud, no subscription, and your chats,
notifications and files never leave the device.

> **Status:** personal project, distributed as a direct APK download
> (see [Releases](../../releases)). It is not on the Play Store.

## What it can do

- **Chat** with an on-device model — fully offline after setup.
- **Cross-app jobs** using Android's own APIs and, where no API exists,
  an accessibility-based "App Driver" (with your approval per action):
  open apps, read the screen, summarize a WhatsApp chat and email it to
  you, and more. Banking/payment/password apps are always out of scope.
- **Email digest & sending** — an unread-mail digest across your
  accounts (IMAP), and direct sending (SMTP) from an account you
  configure. Credentials are stored encrypted with the Android Keystore.
- **Reminders, tasks & routines** — alarms, a morning brief (calendar,
  due tasks, overnight notifications, unread mail), and reactive
  notification rules (e.g. auto-dismiss noisy apps at night).
- **Patterns** — Aura notices routines in your on-device activity log
  and suggests automations. The log never leaves the phone.
- **Photo & video effects** — anime/cartoon styles (several downloadable
  neural styles), face pixelate / blur / emoji for privacy before
  sharing. Originals are never modified; results go to
  Pictures/Aura and Movies/Aura.
- **Device Care** — storage overview, exact-duplicate photo/video
  finder (deletes only through the system's trash consent), battery
  awareness.
- **Floating bubble** — talk to Aura over any app (optional, off by
  default).

## Requirements

- Android 8.0+ (the app is built for modern phones).
- **A recent flagship-class phone is strongly recommended** for the AI
  model (developed and tested on a Galaxy S26 Ultra). On weaker phones
  the model will be slow or may not load.
- ~2.4 GB free space for the model download, plus ~90 MB for the app.

## Getting started

See [INSTALL.md](INSTALL.md) for step-by-step installation and setup.

On first launch Aura runs in a clearly-labelled **demo mode** until you
download the real model (Settings → Model → Download). The download is
~2.34 GB — use Wi-Fi.

## Privacy

Aura is local-first by design. See [PRIVACY.md](PRIVACY.md) for exactly
what the app can access, which permissions it asks for and why, and the
only network calls it ever makes (the model/style downloads you tap).

## Updates

New versions are published as GitHub Releases. Download the newer APK
and install it over the existing one — your data carries over. All
release APKs are signed with the same release key; Android will refuse
an update that isn't, which is your protection against tampered copies.

Verify a download: the SHA-256 checksum is printed in each release's
notes.
