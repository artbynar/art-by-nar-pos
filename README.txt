ART BY NAR POS — BOOKING / DEPOSIT / TRANSACTION UPDATE

Files included:
- index.html: updated POS app
- sw.js: bumped service worker cache version so devices can fetch the new app shell

Install/update on GitHub:
1. Back up POS data from Settings > Export Backup on each device before updating.
2. In the GitHub repository, replace the existing index.html with this index.html.
3. Replace the existing sw.js with this sw.js.
4. Commit changes to the main branch.
5. Wait for GitHub Pages to deploy, then refresh the website on devices.

Features:
- Client name field suggests saved customer names; matching profile details are previewed.
- New client names used in bookings are saved to Customers.
- Booking has Deposit status option, total price, deposit received, and red remaining balance.
- Booking form can record an incoming or outgoing transaction.
- Incoming transactions appear in Payments; outgoing transactions appear in Expenses.
- Booking transaction history is visible when editing that booking.

Important:
- Existing data is stored in each browser/device and does not sync automatically.
- Keep backups before replacing files or clearing website data.
