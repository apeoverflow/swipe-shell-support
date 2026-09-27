# Privacy Policy — Swipe Shell

**Last updated: 27 September 2026**

Swipe Shell is an SSH client. It connects your phone to servers that you own or
have been given access to. This policy describes what the app does with your
information.

## The short version

Swipe Shell has no account, no backend, and no analytics. Nothing you type,
say, or connect to is sent to us, because there is no "us" to send it to — the
app has no server of its own. Your data goes to the servers you choose to
connect to, and nowhere else, with the one exception described under
**Speech recognition** below.

## What is stored on your device

All of the following is stored on your device only:

- **Server details** — hostnames, ports, usernames, and the aliases you give
  them.
- **Credentials** — passwords and private keys, held in the iOS keychain or the
  Android Keystore. They are never written to ordinary files, never written to
  logs, and never displayed in the terminal.
- **Host keys** — the fingerprint of each server you've chosen to trust, so the
  app can warn you if it ever changes.
- **Your settings** — shortcut bar layouts, terminal theme, font size, and
  similar preferences.
- **Open sessions** — which servers you had connected, so the app can offer to
  reconnect them after it restarts. Terminal output is not saved.

Deleting the app removes all of it.

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
app fetches it over HTTPS from the host where it is published. That request
includes only what any file download includes; no identifier for you or your
device is attached.

## What is not collected

Swipe Shell contains no analytics, no crash reporting, no advertising, and no
tracking of any kind. It does not collect:

- Your identity, email address, or any account information
- Which servers you connect to
- What you type, run, or transcribe
- Usage statistics or device identifiers

No data is sold, shared, or disclosed to anyone, because none is collected.

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

When the app copies something for you — a remote file path after an upload, or
text you select in the terminal — it goes to your system clipboard. Text copied
out of the terminal is cleared from the clipboard automatically after a delay
you can configure, so that terminal output doesn't sit on the pasteboard where
other apps can read it.

## Children

Swipe Shell is a developer tool and is not directed at children.

## Changes to this policy

If this policy changes, the updated version will be published here with a new
date at the top. Material changes will also be noted in the app's release
notes.

## Contact

Questions about this policy can be raised as an issue at
<https://github.com/apeoverflow/swipe-shell-support/issues>.
