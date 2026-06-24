# IronTrunks — offline training & nutrition tracker

A self-contained web app. No build step, no server, no database — your data
lives on your device in the browser's local storage. Works offline once
installed to your home screen.

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
