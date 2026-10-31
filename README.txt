ART BY NAR POS — PIN & BACKUP UPDATE

This is a browser-based prototype, not a production-secure POS system.

WHAT'S NEW
- Optional 4–8 digit PIN prompt when the app is opened.
- Set up/change PIN, lock now, and disable PIN from Settings.
- PIN is stored as a salted SHA-256 hash in this browser, not as plain text.
- Daily backup reminder appears in Settings if no backup has been recorded or the last one is older than 24 hours.
- Export JSON backup and import an existing JSON backup.
- Service-worker cache version bumped so the updated app can be fetched.

IMPORTANT LIMITATIONS
- PIN is only a basic local access barrier. It is not strong security; someone with access to the browser storage or source files may bypass it.
- Backup JSON files are NOT encrypted. Store them securely.
- The reminder checks when the app is opened/settings are viewed; it is not a background push notification.
- Data remains in local browser storage on each device. There is no Windows/iPhone sync.
- Do not use real sensitive customer or payment information until the app has been upgraded and security-reviewed.

HOW TO UPDATE THE LIVE GITHUB PAGES SITE
1. Open your repository: https://github.com/artbynar/art-by-nar-pos
2. For each existing file, open it, click the pencil/Edit button, and replace its contents if editing text files; for binary icons, no change is needed.
   EASIER OPTION: Repository > Add file > Upload files, upload the updated index.html and sw.js from this package, then commit changes. If GitHub asks whether to replace existing files, confirm.
3. Ensure index.html, sw.js, manifest.webmanifest, icon-192.png, and icon-512.png are all in the repository root.
4. Wait 1–3 minutes. On iPhone, close the installed web app fully, reopen it while online, and refresh if possible. If it still shows the old version, open the website in Safari first and reload; service-worker updates can take a short while.
5. Open Settings in Art By Nar POS > Set up PIN. Choose a PIN and confirm it. Save a backup from Settings > Export Backup and keep the JSON file somewhere safe.

NOTE: If you already have real data in the old browser version, export a backup before changing app files. The update is designed to keep the same local storage key, but keep a backup anyway.
