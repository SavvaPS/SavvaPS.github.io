GYMSMITH WEBSITE  (repo: SavvaPS.github.io)

Pages
- https://savvaps.github.io/          home
- https://savvaps.github.io/support/  support page  -> App Store "Support URL"
- https://savvaps.github.io/privacy/  privacy policy -> App Store "Privacy Policy URL"

- https://savvaps.github.io/launch.json  founding-member cut-off date, read by the iPhone app

Founding-member cut-off (launch.json)
- "foundingCutoff": null  means the founding window is still open: everyone who
  downloads counts as a founding member (free forever).
- When the App Store version goes live, set the end of the window, e.g.
    "foundingCutoff": "2026-12-31T23:59:59Z"
  Anyone whose Apple ID first downloaded GymSmith before that moment stays free forever.
- To extend the window, move the date later. Never move it earlier.
- Commit and push; the app picks it up the next time it opens online.

No app code lives here. The app itself stays in the separate "gymbook" repo.

Updating the site
1. Edit the files in this folder.
2. In GitHub Desktop: Commit, then Push origin.
3. GitHub Pages republishes within a few minutes.
