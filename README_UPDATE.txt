Art By Nar POS – UI + Reports Update

Included:
- Apple-platform system font stack (uses iOS system font on iPhone; not an embedded proprietary font)
- Liquid-glass-inspired translucent panels and floating bottom navigation
- Daily, monthly and yearly financial report views
- CSV export for report data
- Follow-up list generated from pending/confirmed bookings, pending payments and customer notes with follow-up keywords; mark done/reopen
- Analysis dashboard: paid income, expenses, net cashflow, pending receivables, booking status, top services and ratios
- Service worker cache version bumped so updated files can replace older cached app shell

Update existing GitHub Pages repository:
1. Back up current app data from Settings > Export Backup on each device first.
2. Extract this ZIP.
3. In https://github.com/artbynar/art-by-nar-pos upload/replace index.html and sw.js at the repository root.
4. Commit changes, wait for Pages deployment.
5. On iPhone, open the website in Safari and refresh. If the installed Home Screen app still shows old UI, open Safari site first; if needed remove the Home Screen shortcut and add it again.

Important limits:
- Data remains local to each browser/device; no PC/iPhone sync.
- Follow-up system is an in-app list only; it does not send automatic SMS, email or push notifications.
- Reports and analysis are calculated from entries currently stored in this browser. They are not audited accounting.
- The UI is Liquid Glass-inspired, not Apple's private native Liquid Glass implementation.
- Exported backup/report files are not encrypted. Do not store real sensitive customer data until a secure production system is implemented.
