# Bowling Brackets

Mobile-first bowling bracket manager for H1/H2/H3 handicap brackets and S1/S2/S3 scratch brackets.

## Current features
- Up to six 8-bowler brackets per night
- Handicap calculation from configurable base/percentage/rounding
- Randomized seeds with 1v8, 4v5, 2v7, 3v6 quarterfinals
- Scratch-score entry for Games 1–3
- Handicap totals calculated automatically
- Handicap ties go to higher scratch; exact ties allow manual winner selection
- Paid-entry tracking and collected-dollar totals
- Automatic champion/history archive
- Individual bracket reset and entire-night reset
- Supabase database with Row Level Security and administrator allowlist

## Hosting
The repository includes a GitHub Pages workflow in `.github/workflows/pages.yml`.

## Security
The browser uses only the Supabase publishable key. Database tables have Row Level Security enabled and require an authenticated email that exists in `public.app_admins`. Never place a Supabase secret/service-role key in this repository.
