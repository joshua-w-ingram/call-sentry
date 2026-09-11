# Privacy notes

Call Sentry has no internet permission. Android will not let it open a network connection.
It cannot upload, sync, report, or phone home. That is the whole privacy policy. The rest of
this page explains what each permission is for.

## Permissions

| Permission | Why | What is read |
|---|---|---|
| Read contacts | Rule 1: a number in your contacts rings. | A yes/no lookup of the calling number. The app never lists or copies your contacts. |
| Read call log | Rule 2: a number you called, or answered, rings. | The numbers in your call log and whether each call was outgoing or answered. |
| Read SMS | Rule 3: a number you texted rings. | The addresses in your Sent box only. Message text is never read. Received-only texts do not count. |
| Call screening role | So Android asks the app about each incoming call before it rings. | The calling number, the caller-ID name the network sent, and the network's spoof check result. |

There is no location, camera, microphone, storage, notification, or network permission.

## What is stored on the phone

- A decision log: one line per screened call with the time, ALLOW or BLOCK, the number, the
  reason, the caller-ID name, and the spoof check result. It lives in the app's private
  folder and in the app's own folder under Android/data so you can copy it off with a
  cable. It rotates at 1 MB. Uninstalling the app deletes both copies.
- Your Allow / Disallow overrides, as a small file in the app's private folder.

Nothing else. No settings sync, no cloud backup (backups are disabled in the manifest).

## What leaves the phone

Nothing. The app has no network permission.

## What the carrier's spam label has to do with it

Nothing. The app never reads it. Legitimate businesses get flagged "Spam Risk" all the time,
and spammers spoof clean numbers all the time. The only question the app asks is whether
you have ever reached out to this number.
