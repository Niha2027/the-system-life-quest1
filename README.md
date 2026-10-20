# THE SYSTEM — Life Quest (PWA project)

A Solo-Leveling-inspired personal quest app with daily/date-specific/monthly/yearly quests, inventory, progress tracking, XP, local saves, export/import, quest timers, and original synthesized ambient music.

## What is included
- `index.html` — complete app UI and interactions
- `manifest.webmanifest` — installable web app metadata
- `sw.js` — offline caching service worker
- `icon.svg` — app icon

## Install on Android
1. Host this folder on a secure HTTPS site (GitHub Pages is a free option).
2. Open the published URL in Chrome on Android.
3. Use the browser menu → **Install app** or **Add to Home screen**.

## Install on a PC
1. Open the published HTTPS URL in Chrome or Edge.
2. Select the install icon in the address bar, or browser menu → **Install THE SYSTEM**.

## Local testing
Service workers do not work from a `file://` URL. With Python installed, open a terminal in this folder and run:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000` on that PC. Localhost testing is not the same as installing on another device.

## Important limitations
- The app is a Progressive Web App project, not a signed Android APK or Windows EXE. It can be installed from a secure hosted URL on Android and PC.
- Progress is stored locally in each browser/device. Use Player → Export my save file and Import save file to transfer data manually. Cloud sync is not configured.
- The built-in music is synthesized in the browser and begins only after you tap Play. Browser audio may pause when the app is closed or backgrounded.
- Random in-app nudges work while the app is open. Reliable scheduled background notifications require a push/notification backend or a native app layer.

## Hosting
Upload all four files to a static HTTPS host. Keep the filenames and relative paths unchanged. GitHub Pages, Netlify, or Cloudflare Pages can serve the folder.
