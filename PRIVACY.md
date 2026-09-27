# Privacy Policy — Swipe Shell

**Last updated: 28 September 2026**

Swipe Shell is an SSH client. It connects your phone to servers that you own or
have been given access to. This policy describes what the app does with your
information.

## The short version

Swipe Shell has no account, no backend, and no analytics. Nothing you type,
say, or connect to is sent to us, because there is no "us" to send it to — the
app has no server of its own. Your data goes to the servers you choose to
connect to, and nowhere else, with the exceptions described under
**Speech recognition** and **Purchases** below.

## What is stored on your device

All of the following is stored on your device only:

- **Server details** — hostnames, ports, usernames, and the aliases you give
  them.
- **Credentials** — passwords and private keys. They are never written to
  ordinary files, never written to logs, and never displayed in the terminal.
- **Host keys** — the fingerprint of each server you've chosen to trust, so the
  app can warn you if it ever changes.
- **Your settings** — shortcut bar layouts, terminal theme, font size, and
  similar preferences.
- **Open sessions** — which servers you had connected, so the app can offer to
  reconnect them after it restarts. Terminal output is not saved.

All of it is held in the iOS keychain or the Android Keystore-encrypted store,
marked as belonging to **this device only**. It is left out of iCloud and
Google backups and is not carried across when you restore or transfer to a new
phone — on a new device you add your servers again.

Deleting the app removes all of it. iOS keeps keychain entries after an app is
deleted, so if you reinstall Swipe Shell, it clears anything a previous
installation left there the first time it opens.

## What leaves your device

**To your servers.** Everything you'd expect from an SSH client: the commands
you type, the keystrokes you send, and any files you upload. These go to the
server you connected to, over the encrypted SSH connection, and to nowhere
else.

**Speech recognition.** Swipe Shell offers two recognisers:

- The **system recogniser** provided by iOS or Android. Depending on your
  device, its settings, and the language, your operating system may send audio
  to Apple or Google for transcription. That processing is governed by their
  privacy policies, not this one.
- An **optional on-device model** you can download in
  **Settings → Dictation**. When this is selected, audio is transcribed
  entirely on your device and no audio leaves it.

If you do not want audio processed off-device, use the on-device model.

**Model downloads.** If you choose to download the on-device speech model, the
app fetches it over HTTPS from GitHub, where the open-source speech-recognition
project publishes it. As with any download, GitHub receives your IP address;
its handling is covered by GitHub's privacy statement. No identifier for you or
your device is attached.

**Purchases.** Subscriptions and the lifetime unlock are sold through the App
Store and Google Play. Apple or Google take the payment and handle your payment
details under their own privacy policies; Swipe Shell never sees them. The app
receives only whether your purchase is active.

## What is not collected

Swipe Shell contains no analytics, no crash reporting, no advertising, and no
tracking of any kind. It does not collect:

- Your identity, email address, or any account information
- Which servers you connect to
- What you type, run, or transcribe
- Usage statistics or device identifiers

No data is sold, shared, or disclosed to anyone, because none is collected.
Because everything is on your device, there is nothing held elsewhere for us to
access, correct, or delete for you — deleting the app deletes it.

## Permissions the app asks for

Each of these is requested only when you first use the feature that needs it,
and the app works without any of them.

- **Microphone** — to record speech while you hold the dictation button.
- **Speech recognition** — to transcribe that audio into text.
- **Camera** — to take a photo for uploading to your server.
- **Photo library** — to select existing photos to upload.
- **Face ID / Touch ID** — to unlock the app, if you turn on app lock. The app
  receives only a yes-or-no answer; your biometric data is handled by the
  operating system and is never available to the app.

## Clipboard

Text you copy yourself — a selection from the terminal, or a remote file path
after an upload — goes to your system clipboard and stays there like anything
else you copy.

A program running on your server can also put text on your clipboard (for
example, copying from a remote editor). Because that text comes from the server
rather than from you, Swipe Shell clears it from the clipboard automatically,
after one minute by default. You can change the delay, or turn clearing off, in
the app's security settings.

## This website

The Swipe Shell website sets no cookies and runs no analytics. It is hosted on
Vercel, which keeps standard server logs (such as IP address and browser type)
to operate the service, and it loads its fonts from Google Fonts, which
receives your IP address when the page loads. Both are governed by those
companies' privacy policies.

## Children

Swipe Shell is a developer tool and is not directed at children.

## Changes to this policy

If this policy changes, the updated version will be published here with a new
date at the top. Material changes will also be noted in the app's release
notes.

## Contact

For privacy questions or requests, email
[apeoverflow@proton.me](mailto:apeoverflow@proton.me). General questions can
also be raised as an issue at
<https://github.com/apeoverflow/swipe-shell-support/issues>, but issues are
public — use email for anything you'd rather not post openly.
