# Goa 2026 · Trip Planner 🌴

One-page trip planner for the squad: master plan + day-wise itinerary, live map with
directions, todo list, and a built-in Claude chatbot that edits the plan for you.
Everything auto-saves in each person's browser (localStorage).

## Publish on GitHub Pages (~2 minutes)

1. Go to **github.com** → click **+** (top right) → **New repository**
   - Name: `gkg` (anything works)
   - Visibility: **Public** (required for free GitHub Pages)
   - Click **Create repository**
2. On the new repo page click **uploading an existing file** → drag `index.html`
   (and this `README.md` if you want) → **Commit changes**
3. Go to **Settings → Pages** (left sidebar)
   - Source: **Deploy from a branch**
   - Branch: **main** / folder: **/ (root)** → **Save**
4. Wait ~1 minute. Your live link:

   **https://YOUR-USERNAME.github.io/gkg/**

Share that link with all 7. Done.

## The chatbot needs an API key

The Trip Assistant (bottom-right 🤙) calls the Anthropic API directly from the browser.
First time anyone opens the chat, it asks for an Anthropic API key:

- Get one at **console.anthropic.com** → API Keys
- The key is stored **only in that person's browser** (localStorage) — it is never in
  the website code or the repo.
- Tap 🔑 in the chat header to change it later.

⚠️ **Never commit an API key to the repo.** Anyone can read a public repo.
Sharing one key with all 7 friends is possible (each pastes it once) but remember
everyone can then spend from your API balance. Set a monthly spend limit in the
Anthropic console.

## Heads-up

- The repo is public → the villa address inside `index.html` is public too.
  If that bothers you, either blank the address before uploading, or use a
  **private repo + GitHub Pro** (Pages on private repos needs a paid plan).
- Saved plans live per-browser. Your phone and your laptop each have their own copy;
  friends each have their own too. (A shared live-sync DB needs a backend —
  Firebase/Supabase — happy to wire that up as v2.)

Built with Leaflet + OpenStreetMap + Claude. Ghumo, khao, bach ke gaadi chalao. 🚙🚙
