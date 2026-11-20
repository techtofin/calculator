FINWISE PWA — INSTALLATION & HOSTING

Files:
- index.html: calculator application
- manifest.webmanifest: install metadata and app icons
- sw.js: offline app-shell cache
- icons/: Android/PWA icons

IMPORTANT:
A Progressive Web App must be served from HTTPS (or localhost). Opening index.html directly from a file manager will not enable installation.

DEPLOY:
1. Upload the entire contents of this folder to an HTTPS website/domain, keeping the folder structure.
2. Ensure manifest.webmanifest and sw.js are served from the same directory as index.html.
3. Open the HTTPS URL in Chrome on Android.
4. Tap the browser menu (⋮) > Install app / Add to Home screen.
   If the in-page Install App button appears, you can use that too.
5. Launch Finwise from the new home-screen icon.

OFFLINE:
After the first successful visit, the service worker caches the app shell. Calculators run locally in the browser. The first load needs an internet connection.

This package is a client-side PWA. It does not include user accounts, cloud sync, server-side storage, or regulated financial advice.
