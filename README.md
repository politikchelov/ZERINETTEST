# ZERINET
Stage 1–2 foundation: Next.js 15 + Tailwind 4 + Supabase.

## Run
1. `npm install`
2. Create a Supabase project, run `supabase/migrations/0001_init.sql` then `supabase/seed.sql` in the SQL editor.
3. `cp .env.example .env.local` and fill the URL and anon key.
4. `npm run dev`

## Video
Providers live in `src/lib/video`. Demo provider has no sources by default (honest "no video" state) and is blocked in production unless `ALLOW_DEMO_IN_PRODUCTION=true`.

## Status
Done: design tokens, nav, home/hero, catalog read, schema + RLS (core tables), provider contract.
Stage 2 done: explore (search, filters, sort, pagination via URL), title page, skeleton, 404.
Stage 4 done: native HTML5 player with custom controls (Vidstack not used: untested without network), episodes sidebar, local progress (localStorage; DB sync needs auth).
Not yet: auth, library, community, admin, tests.
