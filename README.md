# Goa 2026 · Trip Planner 🌴

One-page trip planner for the squad: master plan + day-wise itinerary, live map with
directions, place search with autocomplete, todo list, and a built-in Gemini chatbot
that edits the plan for you.
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

   **https://gkg-trip.github.io/**

Share that link with all 7. Done.

## The chatbot

The Trip Assistant (bottom-right 🤙) uses Google Gemini. Zero-setup for the group:
share the **magic link** in the group chat —

`https://gkg-trip.github.io/#k=<GEMINI_API_KEY>`

Anyone who opens it gets the key saved silently in their browser (the `#…` part never
leaves the device and never appears in this repo). Alternatively tap 🔑 in the chat
header and paste a key manually (free at **aistudio.google.com**).

⚠️ Never commit the actual key to this public repo — GitHub blocks such pushes anyway.
Share the magic link only in the private group chat.

## Heads-up

- The repo is public → the villa address inside `index.html` is public too.
  If that bothers you, either blank the address before uploading, or use a
  **private repo + GitHub Pro** (Pages on private repos needs a paid plan).
- Saved plans live per-browser. Your phone and your laptop each have their own copy;
  friends each have their own too. (A shared live-sync DB needs a backend —
  Firebase/Supabase — happy to wire that up as v2.)

Built with Leaflet + OpenStreetMap + Photon + Gemini. Ghumo, khao, bach ke gaadi chalao. 🚙🚙
