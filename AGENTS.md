I'm working on my personal feed website.

Repository: https://github.com/julianboyce/personal-feed

Production: https://personal-feed-phi.vercel.app/

The website is a static frontend hosted on Vercel, reading content directly from Supabase.

Supabase project ID: `hcacxbmiyiaokmkkcwkc`

Supabase URL: `https://hcacxbmiyiaokmkkcwkc.supabase.co`

The database contains a `public.feed_items` table with:

- `id`: uuid, primary key
- `title`: text, required
- `url`: text, required, unique
- `source`: text
- `summary`: text
- `image_url`: text
- `content_type`: text (`article`, `video`, `social_post`, `other`)
- `category`: text
- `published_at`: timestamptz
- `created_at`: timestamptz
- `is_published`: boolean

The frontend can publicly read rows where `is_published = true`.

Please inspect the existing repository and understand the architecture before making changes.

Preserve the Supabase integration, avoid exposing secret keys, and keep the website compatible with Vercel deployment.

Start by explaining the existing structure and recommending improvements. Do not modify anything yet.