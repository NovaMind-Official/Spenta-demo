# SPENTA — Live Demo

This repository hosts a **live, click-through demo** of the SPENTA
marketplace template — a multi-language (FA / EN / DE / FR / ES / TR)
marketplace front-end with category browsing, listing detail pages, a
post-ad flow, wishlist, saved searches, an admin approval queue, seller
profiles, and an interactive 3D globe view.

**This repo contains only the demo build (`index.html`) — not the
project source code.** The source is sold separately.

## View the live demo

Enable GitHub Pages for this repo (**Settings → Pages → Source: Deploy
from a branch → `main` / root**), then visit:

`https://<your-username>.github.io/<this-repo-name>/`

Or open `index.html` directly in any browser — it works standalone,
with no build step or server required.

## What's in this demo

- All 6 categories (Real Estate, Vehicles, Motorcycles, Jobs, Goods &
  Services) with a small sample of listings (~5–6 per category, not
  the full catalog)
- Listing detail pages, filters, search, wishlist, seller profiles
- Sign up / log in (demo mode — phone verification code is `0000`)
- Interactive 3D globe view
- Live currency, gold, and cryptocurrency prices
- Light/dark mode, 6 languages

## What's held back for the full version

This is a limited demo — it showcases the look and core browsing
experience only. Several tools are visible in the menu but intentionally
don't open:

- **Posting an ad** — reachable, but shows a "full version only" message.
- **Compare** — locked with a "full version only" message.
- **Saved searches** — locked with a "full version only" message.
- **Dashboard** (profile / manage my listings) — locked with a "full
  version only" message.
- **Chat with a seller** — the message box works, but sending shows a
  "full version only" notice instead of actually sending.
- **Posting a review** — same pattern: form works, submitting shows a
  notice instead of saving.
- **Identity verification** — clearly labeled "Demo" and the ID photo
  upload is disabled; the rest of the flow still runs as a simulation.
- **Admin approval queue** — visible in the menu, opens to a "full
  version only" message instead of the real moderation workflow.
- Listing photos carry a small "DEMO" watermark.
- A banner across the top, and one at the top of the login/signup form,
  link to the full source purchase page and disclose that accounts/SMS
  are simulated.

The full catalog, and every tool above, are in the full source.

## User accounts in this demo

Sign-up/login works and is real React state, but it's **not a real
account system** — there's no password check and nothing is sent to a
server. Whatever you enter is stored only in your own browser
(`localStorage`), and phone verification always accepts `0000`. This
lets visitors click through the logged-in experience (wishlist, saved
searches, seeing the post-ad and admin gates) without a backend.

## Before you publish this

Open `index.html`, search for `REPLACE_WITH_YOUR_PURCHASE_LINK` (it
appears twice — top banner and the post-ad gate), and replace it with
your actual Codester (or other marketplace) listing URL.

## What's simulated (demo limitations)

This is a front-end-only build, so:

- Accounts and posted ads (if any were saved before gating) are stored
  in **your own browser only** — nothing is shared between visitors or
  persisted on a server.
- Phone/ID verification is UI only, not a real check.
- Listing photos are generated placeholder graphics, not real photos.

## Interested in the source code?

The full React + Vite source (fully customizable — colors, fonts,
categories, translations, branding) is available for purchase. Contact
[your contact info / marketplace listing link here].
