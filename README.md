# AVR REAL ESTATE — Production Starter

Production starter for AVR REAL ESTATE, focused on Puttaparthi.

## Includes
- Premium responsive public website
- Live Supabase property listings
- Property detail pages
- Supabase email/password admin login
- Add/edit/delete property listings
- Database Row Level Security
- Supabase Storage bucket preparation
- WhatsApp enquiry links
- Vercel-ready Next.js project

## Setup
1. Create a Supabase project.
2. Open SQL Editor and run `supabase/schema.sql`.
3. In Authentication → Users, create your admin email/password.
4. Copy that user's UUID and run:
   `insert into public.admin_users (id) values ('YOUR-UUID');`
5. Copy `.env.example` to `.env.local` and enter your Supabase URL, publishable key, WhatsApp number and site URL.
6. Run `npm install` then `npm run dev`.
7. Open `/login` for the private admin panel.
8. Push to GitHub and import into Vercel; add the same environment variables.

The admin form currently accepts image URLs. The Supabase Storage bucket and policies are prepared for native uploads in the next upgrade.
