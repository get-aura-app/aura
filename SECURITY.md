# Security

Aura runs on-device with powerful permissions (notifications,
accessibility), so security reports are taken seriously.

## Reporting a vulnerability

Please report privately — do not open a public issue:

- Use GitHub's private reporting: **Security → Report a vulnerability**
  on this repo, or go directly to
  https://github.com/get-aura-app/aura/security/advisories/new

Include what you found, the Aura version, your phone/Android
version, and steps to reproduce if you have them.

## Supported versions

Only the latest release is supported. Fixes ship in new releases;
there are no patches for older versions.

## Scope notes

- Release APKs are signed with the project release key. An APK from
  anywhere else is not from this project — the SHA-256 in each
  release's notes lets you verify your download.
- Aura's mail feature uses app passwords you create; your account
  password is never requested or stored.
