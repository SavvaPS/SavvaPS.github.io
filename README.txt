GYMSMITH WEBSITE  (repo: SavvaPS.github.io)

Pages
- https://savvaps.github.io/          home
- https://savvaps.github.io/support/  support page  -> App Store "Support URL"
- https://savvaps.github.io/privacy/  privacy policy -> App Store "Privacy Policy URL"
- https://savvaps.github.io/terms/    terms of service -> Google Play "Terms of Service" and the App Store licence agreement

- https://savvaps.github.io/launch.json  founding window and the Android purchases switch, read by the apps

Founding-member cut-off (launch.json)
- "foundingCutoff": null  means the founding window is still open: everyone who
  downloads counts as a founding member (free forever).
- The founding window is 2 weeks. When the App Store version goes live, set the end
  of the window to launch day + 14 days, e.g. "foundingCutoff": "2026-12-31T23:59:59Z"
  Anyone whose Apple ID first downloaded GymSmith before that moment stays free forever.
- To extend the window, move the date later. Never move it earlier.
- Commit and push; the app picks it up the next time it opens online.

Android (launch.json)
- "androidStore": false  keeps the trial and unlock switched off on Android, so everyone
  (including the closed testers) has the full app. Set it to true on Android launch day.
- "foundingStart": null  means no Android founders yet. On launch day set it to the launch
  moment, e.g. "foundingStart": "2026-12-10T00:00:00Z". Android founders are people who first
  install between foundingStart and foundingCutoff, so installs during testing don't count.
  (The iPhone app ignores foundingStart.)
- Launch-day checklist: foundingStart = launch day, foundingCutoff = launch day + 14 days,
  androidStore = true. Commit and push.

No app code lives here. The app itself stays in the separate "gymbook" repo.

Updating the site
1. Edit the files in this folder.
2. In GitHub Desktop: Commit, then Push origin.
3. GitHub Pages republishes within a few minutes.
