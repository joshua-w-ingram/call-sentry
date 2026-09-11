# Call Sentry

Your phone rings only for people you already know. Everyone else goes straight to
voicemail, silently.

I was getting hundreds of spam calls a day. My phone's own spam filter was missing from my
build, and the ones you can download want a subscription and a copy of your contacts. So I
built a filter that never looks at a spam database, never phones home, and never asks me to
do anything.

## The rule

A call rings if the number is one of three things:

1. In your contacts.
2. Someone you called, or answered before.
3. Someone you texted.

That is the whole rule. If you have never reached out to a number, it does not ring. It is
rejected before your phone makes a sound. No missed-call badge, no notification, no entry in
your call log. The caller lands in your voicemail, so a real person can still leave a message.

## What it never does

- No spam database. The carrier's "Spam Risk" label is ignored.
- No internet permission. The app cannot send anything anywhere, and Android enforces that.
- No account, no ads, no analytics, no crash reporting.
- No "they called three times so it must be real". Spammers call three times on purpose.

See [docs/PRIVACY.md](docs/PRIVACY.md) for the full list, permission by permission.

## If it blocks someone real

Open the app. Every blocked number is listed with the caller-ID name the network sent, the
time, and how many times they tried. Tap **Allow** once and that number rings from then on.
Tap **Disallow** on anyone you want gone, even someone in your contacts.

## Install

It is not on the Play Store. You install the file yourself, which takes about two minutes.
Step by step: [docs/INSTALL.md](docs/INSTALL.md).

Short version: download `CallSentry.apk` from the
[Releases page](https://github.com/joshua-w-ingram/call-sentry/releases), tap it, allow the
install, open the app, tap **1** (permissions) and **2** (make it your call screening app).
Close it. You never need to open it again.

Requires Android 10 or newer. Tested on a Samsung Galaxy S24+ running Android 16.

## Battery

None worth measuring. The app does nothing at all until a call comes in. Android wakes it,
it answers in a few milliseconds, it exits.

## Source

The app source is private. This repository holds the documentation and the releases.

## License

MIT. See [LICENSE](LICENSE).

Call Sentry by [life-h.ac/ked](https://life-h.ac/ked/).
