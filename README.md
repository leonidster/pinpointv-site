# PinpoinTV Landing Page — Deploy Guide

Self-contained, mobile-responsive landing page. No build step, no dependencies. Just HTML + your real assets.

## What's here
- `index.html` — the page (brand colors, hero, embedded YouTube demo, 3-step how-it-works, screenshot carousel, feature grid, CTAs).
- `assets/` — your real icon, feature graphic, and 5 app screenshots.

## Before you publish — fill in 4 links
Open `index.html` and replace every `href="#"` marked `<!-- TODO -->` with your real **Google Play listing URL**. There are 4 spots:
1. Hero "Get it free on Google Play" button
2. Bottom band "Get PinpoinTV free" button
3. Footer "Google Play" link
4. Footer "Feedback" link → paste your Google Form URL (see plan Phase 0)

Tip: in a text editor, find-and-replace `href="#"` → your Play URL all at once, then fix just the Feedback one.

## Deploy free — GitHub Pages (recommended, ~5 min)
1. Create a public repo, e.g. `pinpointv-site`.
2. Upload the **contents** of this `site/` folder (so `index.html` is at the repo root, `assets/` beside it).
3. Repo → **Settings → Pages** → Source: `main` branch, `/ (root)` → Save.
4. Your URL appears in ~1 min: `https://<username>.github.io/pinpointv-site/`.

### Or Netlify / Cloudflare Pages (drag-and-drop)
- Netlify: drag the `site/` folder onto https://app.netlify.com/drop — instant URL.
- Both give a free `*.netlify.app` / `*.pages.dev` domain; add a custom domain later if you want.

## Notes
- **The embedded video** will only play once the page is served from a real `http(s)` URL **and** the YouTube video `w4Oy2HNAvKk` is set to **Public** (Unlisted also works for embeds). It will NOT play from a local `file://` open — that's expected.
- The page is already SEO + social-share ready (title, meta description, Open Graph image = your feature graphic).
- This is your **link-in-bio** destination for every social profile (TikTok, IG, X, Reddit, YouTube).
