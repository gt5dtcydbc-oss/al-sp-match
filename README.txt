# Anime Releases Tracker PWA

Files included:
- `index.html` - your app, patched for PWA installability
- `manifest.webmanifest` - install metadata
- `service-worker.js` - app shell cache
- `icons/` - generated app icons

## What changed
- Added manifest, theme color, Apple web app meta tags
- Added service worker registration
- Added generated icons for install / home screen
- Added a small iPhone install hint
- Added local snapshot restore so the last loaded state shows before refresh

## How to use on iPhone
1. Upload this folder to a static host over HTTPS
2. Open the site in Safari on iPhone
3. Tap Share
4. Tap Add to Home Screen
5. Open it from the new home screen icon

## Hosting options
Any static HTTPS host works, for example:
- Netlify
- Vercel
- GitHub Pages

## Notes
- The service worker caches the app shell, not live AniList / releases.moe data
- The app still needs internet access to refresh live results
- If releases.moe is blocked in the browser, you still need your proxy option from the page
