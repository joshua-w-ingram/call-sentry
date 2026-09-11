# Installing Call Sentry

Android only. Android 10 or newer. About two minutes. You are installing a file from outside
the Play Store, so Android will warn you a couple of times. That is normal for any app that
is not in the store.

## 1. Download

On your phone, open the Releases page:

https://github.com/joshua-w-ingram/call-sentry/releases

Tap the newest `CallSentry.apk`. Chrome may say "This type of file can harm your device".
Tap **Download anyway**. It is a 70 KB file.

## 2. Open the file

Pull down the notification shade and tap the finished download, or open the Files app and
tap `CallSentry.apk` in Downloads.

## 3. Allow installs from this source

The first time, Android says "For your security, your phone is not allowed to install
unknown apps from this source". Tap **Settings**, turn on **Allow from this source**, then
go back. Tap **Install**.

Samsung phones may add "Blocked by Play Protect" or "Unsafe app blocked". Tap **More
details**, then **Install anyway**. Play Protect flags every app it has never seen; it is not
a finding about this app.

## 4. Open Call Sentry and tap the two numbered buttons

1. **Grant permissions.** Three of them: contacts, call log, and SMS. Each one is a
   read-only look at your own phone so the app can tell who you already know. Tap **Allow**
   on each.
2. **Set as call screening app.** Android asks which app should screen calls. Pick
   **Call Sentry**. The status line under the buttons changes to "Screening role: HELD
   (active)".

That is it. Close the app. You never need to open it again.

## 5. Check on it, if you want

Open the app any time. The top shows how many calls were blocked and allowed today. Below
that, every blocked number with the caller-ID name the network sent, the time, and how many
times it tried. Tap **Allow** on any number that turned out to be real. Tap **Disallow** on
any number you want gone.

## Updating

Download the newer `CallSentry.apk` and install it the same way. Your Allow / Disallow list
stays. If Android refuses with "App not installed", the release was signed with a different
key; that will be called out in the release notes.

## Uninstalling

Long-press the icon, App info, Uninstall. Android hands call screening back to the phone's
own dialer.

## If something is off

If a call you expected did not ring, open the app and look at the blocked list. The
line shows why it was blocked ("unknown" means the number matched none of the three rules).
Tap **Allow** and call them back. If nothing is being blocked at all, check the status line:
"Screening role: NOT HELD" means step 2 did not stick. Tap button 2 again.
