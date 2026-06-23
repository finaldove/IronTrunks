# IronTrunks — offline training & nutrition tracker

A self-contained web app. No build step, no server, no database — your data
lives on your device in the browser's local storage. Works offline once
installed to your home screen.

## Files
- `index.html` — the whole app
- `manifest.webmanifest` — makes it installable to the home screen
- `sw.js` — service worker (offline caching)
- `icon-192.png`, `icon-512.png` — app icons

Keep all files together in the same folder / repo root.

## Put it online (GitHub Pages — free, one time)
1. Create a free GitHub account if you don't have one.
2. Create a new **public** repository, e.g. `irontrunks`.
3. Upload these files to the repo root (drag them into the "Add file → Upload
   files" page, commit).
4. Repo **Settings → Pages**. Under "Build and deployment", set Source =
   *Deploy from a branch*, Branch = `main`, folder = `/ (root)`. Save.
5. Wait ~1 minute. Your app is live at:
   `https://YOUR-USERNAME.github.io/irontrunks/`

## Install on your phone
**Android (Chrome):** open the URL → menu (⋮) → **Add to Home screen / Install
app**. It lands on your home screen and opens like a normal app.

**iPhone (Safari):** open the URL → Share → **Add to Home Screen**.

After installing, it runs offline. Log whenever, close it, reopen — your data
stays.

## Backups
Stats tab → **Export** saves all your data to a JSON file. **Import** restores
it. Export before any app update, and now and then for safety (especially on
iPhone, where the system can clear an unused app's storage).

## Updating later
Replace `index.html` (and bump the cache name in `sw.js`, e.g. `-v2`) in the
repo. Export your data first, update, then Import if anything looks empty.
Your logged data is stored separately from the app files, so updates don't
erase it.
