ATHLETE OS — Progressive Web App package

FILES
- index.html: the app
- manifest.webmanifest: install/app metadata
- sw.js: offline service worker
- icons/: app icons for Android/iOS-compatible installation flows

BEST PHONE SETUP
1. Upload this folder to a static HTTPS host such as GitHub Pages, Netlify, Vercel, Cloudflare Pages, or similar.
2. Open the HTTPS site on your phone.
3. Android/Chrome: use the browser menu and choose Install app / Add to Home screen.
4. iPhone/Safari: Share -> Add to Home Screen.
5. The app can then launch in standalone mode and retain the local training data stored by that browser.

IMPORTANT DATA NOTE
Workout data uses browser localStorage. Export the app's JSON backup periodically, especially before changing devices or browsers.

The service worker requires HTTPS (or localhost) to register. Opening index.html directly with a file:// URL still lets you use the app, but it will not provide full PWA installation/offline-service-worker behavior.
