---
title: Privacy policy
---

# Privacy policy: H743 app


**Who we are:** Mithun Kamat, Pune, India, contact mithun.kamat@gmail.com. This policy covers the
Android app "H743" (`com.mkamat.h743app`) and the cloud service it uses.

**What the app does:** it shows the status of your H743 boards and lets you control them, through our cloud service on
Amazon Web Services (AWS, region Asia Pacific, Mumbai) or directly over Bluetooth next to a board.

## What we collect and why

| Data | Why | Kept |
|---|---|---|
| Your **e-mail address** and a **password** (the password is stored only as a hash by Amazon Cognito; we never see it) | to create and sign in to your account; e-mails with sign-up and reset codes | until you delete your account |
| An **account id** and an **identity id** made by Amazon Cognito | to link you to your boards and your rights on them | until you delete your account |
| Your **rights on boards** (owner, service, operator, viewer) | to decide what you may see and do | until you or the board owner remove them, or you delete your account |
| An **install id** (a random number made by the app on your phone) | to allow one phone per account at a time | until you delete your account (the active one); on the phone until you uninstall the app |
| **Commands you send** to a board (which, when, from whom) | to send the board's answer back only to you | deleted when the board answers |
| **Board status** (firmware version, uptime, temperature, LED state, Wi-Fi signal) | to show it to the users of that board | not stored by us beyond the board's last status (AWS IoT "shadow") |
| On the phone: a 24-hour history of the readings | the graph in the app | on your phone only; removed with the app |

We do **not** collect your location. On Android 11 and older Android itself asks for the location permission before an
app may search for Bluetooth devices; the app uses it only for that search and never reads or stores a location. We do
not use advertising, analytics or tracking, and we do not sell or share your data. Our processor is Amazon Web
Services (Cognito, API Gateway, Lambda, DynamoDB, IoT Core, KMS), which stores the data above for us in the AWS region
named above.

**Security:** all connections are encrypted (HTTPS / TLS); commands to a board are signed in AWS and checked by the
board; optional two-step sign-in (an authenticator app) is required to own a board.

## Your choices and rights

- **Delete your account** in the app (menu → "Delete my account…") or at https://mithunkamat.github.io/H743_AppPages/delete-account.html: your sign-in,
  your account and identity ids and all your board rights are deleted at once; boards you owned can then be claimed
  again. Board status that a board sends on its own is not personal data of yours.
- Ask us for a copy of your data or a correction: mithun.kamat@gmail.com.
- Children: the app is meant for adults, not for children.

**Changes:** we will publish changes here with their date. Last change: 2026-11-24.
