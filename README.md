# Swipe Shell — Support

Swipe Shell is an SSH client for iOS and Android, built for phones rather than
for a keyboard you don't have.

This repository is where support for the app lives. The app's source is not
here — only the things you need to get help, report a problem, or read what the
app does with your data.

- **[Report a bug or ask a question →](https://github.com/apeoverflow/swipe-shell-support/issues/new)**
- **[Privacy policy →](PRIVACY.md)**

## Getting help

Open an issue. It's the fastest route and it's read by the person who wrote the
app. There's no account requirement beyond a free GitHub account.

When reporting a bug, the following makes it much easier to fix:

- What you were doing, and what happened instead
- Your device and iOS/Android version
- The app version, from **Settings → About** (or the App Store listing)
- Whether the server is macOS or Linux, and whether you're running a
  multiplexer such as tmux
- If it's a rendering problem, what program was on screen — a shell, an editor,
  a full-screen TUI

**Never paste a password, a private key, or the contents of a terminal session
into an issue.** Issues here are public. If something can only be explained by
showing sensitive output, say so in the issue and we'll find another way.

## Common questions

**The app asks for a host key to be trusted. Should I?**
Only if you recognise the fingerprint. Swipe Shell shows you the server's key
fingerprint the first time you connect and remembers it. If it ever changes,
the app refuses to connect and does not send your credentials — that warning is
the one thing you should never click past without understanding why the key
changed.

**Dictation isn't producing text.**
Check that microphone and speech-recognition permission are granted in your
device settings. The system recogniser needs both. If you've downloaded the
on-device model, check it's still installed under **Settings → Dictation** —
deleting and reinstalling the app removes it.

**I reinstalled the app and the dictation model is gone.**
Deleting an app removes everything it stored, including the model. A normal
App Store update does not. The model has to be downloaded again after a
reinstall.

**My session dropped and came back with a fresh shell.**
A dropped SSH connection means the remote shell and everything it was running
are gone. To have sessions genuinely survive, run a multiplexer such as tmux on
the server and set it as the host's startup command — Swipe Shell will reattach
to it instead of starting a new shell, and your screen comes back as you left
it.

**Does Swipe Shell change anything on my server?**
No. It never writes to `.tmux.conf`, `.vimrc`, or any other file on the host,
and it never probes to work out what you're running. It runs the command you
configured and nothing else.

## Security

If you believe you've found a security vulnerability, please **do not** open a
public issue. Report it privately through GitHub's
[security advisory form](https://github.com/apeoverflow/swipe-shell-support/security/advisories/new)
so it can be fixed before it's described publicly.
