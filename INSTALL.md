# Installing Aura

Aura is distributed as a direct APK download. Android calls this
"sideloading" — it takes about two minutes.

## 1. Download

1. Open this repo's [Releases](../../releases) page on your phone.
2. Download the `aura-<version>.apk` file from the latest release.
3. (Recommended) Check the SHA-256 in the release notes matches the
   file you downloaded.

## 2. Install

1. Tap the downloaded APK in your browser's downloads (or in the
   Files app → Downloads).
2. Android will say this app can't install apps yet — tap
   **Settings** and allow **"Install via USB / Allow from this
   source"** for your browser or Files app, then go back and tap
   **Install**.
   (This is a per-app permission; you can revoke it afterwards.)
3. Open Aura.

Android may show a Play Protect scan the first time — that's normal
for apps installed outside the Play Store.

## 3. First-run setup

1. **Get the real model (Wi-Fi recommended):** Settings → Model →
   **Download**. It's a one-time ~2.34 GB download of Gemma 4 E2B.
   Until then Aura runs in a labelled **demo mode** with canned
   replies so you can explore the UI.
2. Tap **Load** after the download finishes. The model then loads
   automatically on each start.

## 4. Permissions (all optional, all explained in-app)

Aura asks only for what a feature needs, when it needs it:

- **Notifications access** — lets Aura see incoming notifications for
  the morning brief, patterns and notification rules.
- **Accessibility** — powers the App Driver (reading/driving other
  apps for cross-app jobs). Every write action asks for your approval
  first; banking, payment and password apps are never read or driven.
- **Calendar** — for listing/creating events.
- **Photos & videos** — for attaching media and the Device Care
  duplicate scan.
- **Usage access** — for per-app storage sizes in Device Care.
- **Exact alarms** — so reminders and the morning brief fire on time.
- **Draw over other apps** — only if you turn on the floating bubble.

You can review and fix everything later from Settings, which lists
anything that's missing with a per-item **Fix** button.

## 5. Email (optional)

To use the email digest or send mail from Aura, add an account in
Settings → Email sending with an **app password** from your provider
(for Gmail: Google Account → Security → App passwords — this requires
2-Step Verification). Your regular password will not work, and Aura
never sees it. Credentials are encrypted on-device with the Android
Keystore.

## Updating

Download the newer APK from Releases and install it the same way —
it updates in place and keeps your conversations, rules and settings.
Release APKs are all signed with the same key; if Android ever refuses
an update "because the signature doesn't match," **do not** uninstall
to force it — that file didn't come from here.

## Uninstalling

Uninstall like any app. The downloaded model file (~2.34 GB) lives in
the app's private storage and is removed with it. Photos/videos Aura
created in Pictures/Aura and Movies/Aura stay — they're yours.
