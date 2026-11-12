# Website numbers

One dashboard page, shared by three businesses. Each gets its own link; the
key in the link decides whose numbers appear.

- T M Professional Window Cleaning — newmarketwindowcleaner.co.uk
- KAT Window Cleaning — katwindowcleaning.com
- The Roof & Render Cleaning Company — roofandrendercleaning.com

Open it as `?token=<that business's key>`, and optionally `&days=7|30|90`.

Visits are counted without cookies. The server turns a visitor's address and
browser into a salted hash that changes nightly and cannot be reversed, so no
consent banner is needed and no address is ever stored.

The numbers come from the `stats` function in the foner Supabase project,
which reads the shared `web_*` tables. The tracking script that fills those
tables lives in each site's own repo as `js/analytics.js`.
