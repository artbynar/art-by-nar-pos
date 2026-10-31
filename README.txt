ART BY NAR POS — PWA PACKAGE

This package prepares the current browser prototype for Home Screen installation as a Progressive Web App (PWA).

HOW TO PUBLISH (one-time internet setup)
1. On your Windows PC, sign in to GitHub and create a NEW repository.
2. For the easiest GitHub Pages setup, set the repository to Public. Do not put private customer data in this repository.
3. Upload these files to the repository root: index.html, manifest.webmanifest, sw.js, icon-192.png, icon-512.png.
4. Open repository Settings > Pages.
5. Under Build and deployment, choose Deploy from a branch, select main and / (root), then Save.
6. Wait for the published URL shown on the Pages settings screen. It should be HTTPS.
7. Open that URL on the iPhone in Safari. Tap Share > Add to Home Screen, leave Open as Web App enabled if shown, then tap Add.
8. Open it from the new Home Screen icon once while online so the service worker can cache the app shell. Then test in Airplane Mode.

IMPORTANT
- This is still the existing prototype wrapped as a PWA, not a completed production POS.
- Data is stored locally in each browser/app context. It does not automatically sync between Windows and iPhone.
- Browser storage can be lost; export backups and test restore.
- The prototype's JSON backup is not encrypted. Do not enter real sensitive customer data until the production build has proper security and backups.
- The service worker caches the app shell only; do not assume all features or data are available offline until tested on the actual iPhone.
- A public GitHub Pages site means the app code is public. Do not upload customer records, backups, passwords or secrets.
