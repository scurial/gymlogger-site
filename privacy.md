# GymLogger privacy policy

_Last updated 27 September 2026_

GymLogger is a small app that notices when you are at your martial arts gym and logs the session as a workout in Apple Health. It exists because Jiu Jitsu is a contact sport: you cannot wear a watch or a fitness tracker on the mat, so those sessions never reach Apple Health on their own. GymLogger uses your phone's location instead, so your training is logged automatically without anything on your wrist. This page explains what it collects, where it goes, and how to get rid of it.

## What the app does with your location

GymLogger asks for **Always** location access so that iOS can tell it when you arrive at and leave the gyms you have saved. It does this with geofences: iOS watches the small circles you drew around your gyms and wakes the app at the boundary. The app does **not** track your route, record your position during the day, or know where you are when you are not at a gym.

Once, when the app opens after a possible missed arrival, it takes a single position fix to check whether you are inside one of your gym circles. That fix is compared to your gyms and discarded.

## What is stored on your phone

Everything the app needs lives in one file on your phone: your gyms (name, address, coordinates and radius), your detected and manual sessions (which gym, arrival and departure times, how the session was classified), your settings, and a short log of boundary crossings used for troubleshooting.

## What is written to Apple Health

With your permission, each logged session is saved to Apple Health as a **Martial Arts** workout with an estimated active-energy figure. The app reads your **body mass** from Health to make that estimate, and reads its own **workouts** back to avoid logging a session twice. Health data is never sent anywhere; it stays in Apple Health under Apple's rules, and you can revoke access at any time in Settings › Health › Data Access & Devices.

## What is sent to the cloud

GymLogger keeps a copy of some of your data on a server (Supabase, hosted in the United States) so that it survives a new phone and so the leaderboard can work. Each install gets an anonymous account automatically; you can link Sign in with Apple to make it recoverable.

Synced to your account:

- **Your gyms**, as links to a shared gym catalogue, with your personal radius. The catalogue entry (name, address, coordinates) is visible to every signed-in user, so people at the same gym end up on the same entry; your link to it is not visible to other users.
- **Your sessions**: gym, arrival and departure times, classification, and the identifier of the Health workout.
- **Your settings** (trim, minimum and maximum session length, default class length, usual workout intensity, weight unit, calorie fallback weight, your default gym and the leaderboard you last viewed).
- **Your profile**: a display name and whether you share on leaderboards.

Never synced: your position fixes, the raw crossing log, your body weight, or any Health data beyond the workout identifier above.

Besides the features above, synced data is used to maintain the shared gym catalogue and to understand how the app is used, for example how many accounts are created. Nothing extra is collected for this.

If you link Sign in with Apple, Apple sends the app your name and an email address (or a private relay address, if you choose "Hide My Email"). The name is used to pre-fill your display name once; the email is held by the authentication service as your login. It is not shown to other users.

## Leaderboards

Sharing on leaderboards is **on by default** and can be turned off in Settings › Leaderboard. When it is on, your **display name, session count and current streak** appear on the board of each gym you trained at, and on the boards for that gym's city, metro area, state and country. Any signed-in user can open the board for any gym or place, not only the ones they train at. On boards wider than a single gym, your row also names the gym where you trained most in the period the board covers, so someone looking through the boards can tell which gyms you have trained at. Other users cannot see when you trained, which sessions you had, or anything else. When sharing is off, you can still see the boards; you just do not appear on them. Your display name defaults to "Anonymous" until you change it or link Sign in with Apple.

## Diagnostics you choose to send

Settings › Diagnostics › Share diagnostics builds a file containing the app's state, permissions, your gyms, sessions and crossing log, and hands it to the iOS share sheet. Nothing is sent unless you choose a recipient. If you send it to the developer, it is used only to work out what went wrong, and deleted once that is done.

## What is not collected

No analytics SDKs, no advertising identifiers, no third-party trackers, no crash-reporting service beyond what Apple's TestFlight and App Store provide with your consent.

## Deleting your data

- Deleting the app removes everything stored on the phone. Workouts already written to Apple Health remain there and can be deleted in the Health app.
- To delete your cloud account and everything synced to it, email the address below from the device with the app installed and quote the account identifier shown in Settings › Account. It will be removed within 30 days. An in-app "Delete account" button is planned.
- Gyms you added to the shared catalogue stay in it, no longer linked to you. A record that an account with your identifier was deleted, and when, is kept, together with when the account was created and whether it was anonymous; it does not include your email.

## Contact

gymloggerphoneapp@gmail.com

## Changes

If this policy changes, the date at the top moves and the app's release notes say so.
