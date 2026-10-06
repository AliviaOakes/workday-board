# Alivia's Workday Board

Daily work log, weekly rhythm, bug tickets, personal routine, home upkeep and money ledger.

- **Site:** https://aliviaoakes.github.io/workday-board/
- **Data:** Supabase (project `ajhrvcriyznwhljyuonu`). Sign-in is by emailed link; only emails in the `members` table can read or write.
- **Add someone:** in Supabase → Table Editor → `members`, add a row with their email and role (`owner`, `editor` or `viewer`).

Everything lives in `index.html`. The key in it is Supabase's publishable key, which is meant to be public; access is enforced by the database's row-level security.
