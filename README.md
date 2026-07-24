# Comeback Blueprint PWA

## Install on iOS 26

This app must be served from an HTTPS website. Opening `index.html` directly
from the Files app does not allow the service worker to register.

1. Upload the complete folder contents to an HTTPS static host.
2. Open the resulting URL in Safari on the iPhone.
3. Tap Share.
4. Tap Add to Home Screen.
5. Launch Comeback Blueprint from its Home Screen icon.

## Easy hosting choices

- GitHub Pages
- Cloudflare Pages
- Netlify
- Vercel
- Any ordinary HTTPS web server

Keep the directory structure intact. `index.html`, `sw.js`,
`manifest.webmanifest`, and the `icons` folder must share the same site root.

## Data

Workout data remains in the browser's localStorage. It is device/browser
specific. Use Export data inside the app to make backups.

## Offline updates

The service worker caches the app shell after the first successful hosted
load. To release a future version, change `CACHE` in `sw.js`, for example
from `comeback-blueprint-v1` to `comeback-blueprint-v2`.
