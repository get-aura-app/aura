# Aura privacy

Aura is a local-first assistant. This page describes, plainly, what
the app can access and what leaves your phone (almost nothing).

## The short version

- **No account. No analytics. No ads. No telemetry.** Aura has no
  server to phone home to.
- The AI model runs **on your device**. Your prompts, conversations,
  notifications, activity log and files are processed and stored
  locally.
- There is **no cloud fallback**. If a question needs the live web,
  Aura says so instead of sending your data anywhere.

## What stays on your phone

- Conversations, tasks, reminders, rules and settings
  (app-private storage).
- The activity log used for pattern suggestions (capped, on-device).
- A mirror of your current notification shade (for the brief,
  digests and rules) — on-device only.
- Email credentials, if you configure email — encrypted with the
  Android Keystore and used only to talk to *your* mail provider.

## Network calls Aura makes

Only ones you initiate:

1. **Model download** — the Gemma 4 E2B model file (~2.34 GB) from
   Hugging Face, when you tap Download in Settings.
2. **Style downloads** — small anime-style model files from Hugging
   Face, when you tap Download next to a style.
3. **Your email** — IMAP/SMTP connections to the provider of any
   account *you* configure, using the app password *you* entered.
   Sending an email is, obviously, a network action you asked for.

Nothing else. In particular, Aura never uploads your chats, photos,
notifications or activity log anywhere.

## Permissions, honestly

Each permission unlocks a feature and is requested in context (see
INSTALL.md for the list). The strongest ones — notification access
and accessibility — exist so Aura can do jobs *for you on your
phone*, under an approval system: read-only actions proceed,
writes ask, and irreversible actions always ask. You can pause Aura
globally or disable individual tools, and every action is written to
an on-device audit log.

Banking, payment, wallet, password-manager and authenticator apps
are hard-blocked: Aura will not read or drive them, and never reads
one-time codes.

## If you stop using Aura

Uninstalling removes the app and everything in its private storage,
including the model and any stored email credentials. Media Aura
created for you in Pictures/Aura and Movies/Aura remains, like any
of your files.
