# Art By Nar Premium POS — Starter v1
Responsive Luxury Dark + Gold POS starter for iPhone and Windows.

## Includes
- Dashboard, customers, bookings, and transaction ledger
- Booking deposit and remaining-balance calculation
- Booking deposit automatically creates a Money In transaction
- Supabase cloud database and email/password sign-in integration

## Setup required before it works online
1. Create a project at https://supabase.com/.
2. In Supabase SQL Editor, run `supabase_schema.sql`.
3. In Supabase Project Settings → API, copy the Project URL and anon/publishable key.
4. In `index.html`, replace `YOUR_SUPABASE_PROJECT_URL` and `YOUR_SUPABASE_ANON_OR_PUBLISHABLE_KEY`.
   Never use the `service_role` / secret key in browser code.
5. Enable Email authentication and create trusted staff accounts under Authentication → Users.
6. Deploy `index.html` to the GitHub Pages root, then sign in.

## Security / limitations
This first starter uses a shared single-studio workspace: every authenticated user can read/write all studio records. Only create trusted staff accounts. Review roles and RLS before production. Edit/delete tools, audit history, customer linking, backups and booking conflict checks are future hardening steps. This file is not yet connected to your Supabase project or deployed. Test with dummy records before real business use.
