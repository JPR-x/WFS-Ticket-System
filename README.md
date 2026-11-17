# WFS Ticket System (demo)

Concept prototype for digital ticketing: loading/unloading tickets, supplemental crew tickets, AMS services, roster and schedule, incident and corrective-action reports.

**Demo only. All data is fictional.** Sign-in is client-side and data is stored in each browser. Not for production use.

## Demo accounts
- MOD: `mod` / `MOD2026`
- Supervisor: `sup` / `SUP2026`
- Administrator: `admin` / `ADMIN2026`

## Run locally
Open `index.html` in a browser, or serve the folder:

    python3 -m http.server 8000

Then visit http://localhost:8000. Offline use and home-screen install need the app served over HTTPS or localhost.

## Files
- `index.html`: the whole app (HTML, CSS, JavaScript)
- `manifest.webmanifest`, `sw.js`, `icons/`: installable app and offline cache

## Updating
Change `CACHE` in `sw.js` (e.g. `wfs-ops-v2`) whenever `index.html` changes, so devices fetch the new version.
