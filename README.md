# SHRI Workforce Website

Public website for SHRI manpower services in Mumbai. This repository is published with GitHub Pages.

## Live pages

- **Home:** [index.html](index.html)
- **About:** [about.html](about.html)
- **Services:** [services.html](services.html)
- **Contact:** [contact.html](contact.html)
- **Privacy policy:** [privacy.html](privacy.html)
- **My Account:** [myaccount.html](myaccount.html) — current Supabase-based login and account dashboard.

The live account page is available at:
https://1sam1.github.io/Shri-website-/myaccount.html

## Repository layout

- `*.html` — website pages.
- `css/style.css` — shared site styles.
- `js/script.js` — shared site scripts.
- `images/` — logos, service images, and team images.
- `Shri.apk` — Android application package currently stored in the repository.
- `My Account1` — separate older workforce-parser entry page (filename has no extension). Review its current purpose before renaming or removing it.

## Editing and publishing

1. Make changes on a branch and review them before merging into `main`.
2. Keep existing page filenames and relative links stable unless all references and live URLs are checked.
3. Preview changes on GitHub Pages after merging.
4. Do not commit passwords, service-role keys, service-account JSON, bot tokens, or other private credentials.

## Supabase account page security

The current `myaccount.html` uses the Supabase JavaScript client in the browser. A publishable/anonymous client key is intended to be public; it is **not** an authorization boundary. Access to profiles, employees, shifts, advances, payments, and reviews must be enforced by correct Supabase Row Level Security (RLS) policies and role-specific database permissions. Never put a Supabase service-role key in this repository. Verify RLS and role-based access before using real employee or customer data.

## Cleanup notes

The legacy `My Account1` and `Shri.apk` remain in the repository. Confirm whether each is still used before renaming or deleting it. The old `test.html` dashboard has been deleted because it read published Google Sheets CSV feeds and should not be treated as a secure login system.
