# Personal Feed

Static, responsive website that reads published articles from Supabase.

## Deploy

Import this directory as a static site in Vercel (Framework Preset: Other, no build command, output directory: `.`), or deploy via Vercel CLI (`vercel --prod`).

The frontend uses a public Supabase publishable key. Row Level Security must remain enabled on `public.feed_items`, and public access should be SELECT-only for published records.

Adding a new published record to `feed_items` makes it visible on page refresh without rebuilding.
