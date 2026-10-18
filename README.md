# Koya local copy (snapshot of koya.living, 17 Oct 2026)

Run: open this folder in VS Code and use Live Server, or run `python3 -m http.server 8000` and open http://localhost:8000/index.html

- index.html and reserve.html hold all the real CSS and JavaScript (inline).
- styles.css and script.js are an old version. index.html does not use them.
- On localhost the page reads api/menu, api/sections, api/gallery and mock-menu.json from this folder. These are a snapshot of the live data (114 items, 21 sections).
- Photos: koya_bg/, koya_pics/, koya_menu_pics/, uploads/.
- reserve.html always posts to https://koya.living. Do not press Submit while testing.
- Google sign-in does not work on localhost.
- If edits do not show, open DevTools, Application, Service Workers, and turn on Bypass for network.
- mock-menu.old.json is the sample that came in the original zip.

## Local assets update, 18 Oct 2026

- Added the missing twelfth gallery photo: uploads/fcc9cf28-4dbc-4c2d-af38-f5cb461e5b4e.webp. All 12 gallery references now have local files.
- Bundled Bootstrap 5.3.0, Font Awesome Free 6.4.0 (CSS and webfonts), Poppins weights 300/400/500/600/700, and Kaushan Script. Both HTML pages now load these from vendor/.
- Bundled the reservation page background that previously loaded from Pexels.
- Included upstream licenses and asset-sources.json.
- The original 12 menu items without image references still have no dish photos; no substitute photos were added.
- This is a local presentation snapshot. Reservation submissions and Google authentication still require the live services described above.
- Use a new localhost port (e.g. python3 -m http.server 8001) if the old service worker shows cached files.
