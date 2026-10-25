RIGHT NOW — MOBILE-READY PWA PACKAGE

Files:
- index.html: mobile-responsive Right Now app
- manifest.webmanifest: installable PWA metadata
- sw.js: basic app-shell caching for supported browsers
- icon.svg: app icon

LOCAL DESKTOP TEST
1. Extract this folder.
2. Open it in VS Code.
3. Install the VS Code Live Server extension if needed.
4. Right-click index.html > Open with Live Server.

PHONE TEST / INSTALL
1. Deploy the folder to an HTTPS host (for example Firebase Hosting).
2. Open the deployed HTTPS address in Chrome on Android or Safari on iPhone.
3. Android: browser menu > Install app / Add to Home screen.
4. iPhone: Safari Share button > Add to Home Screen.

IMPORTANT
- Browser location permissions generally require HTTPS (or localhost for development).
- The app uses Firebase Realtime Database configured in the HTML. Real-time features require internet access and correctly configured Firebase database rules.
- This package does not itself deploy the app or configure Firebase security rules.
- This is a prototype and does not automatically contact emergency services. Do not rely on it as the only way to seek urgent help; call local emergency services directly when needed.
- The service worker caches the app shell, but external CDN libraries and Firebase real-time features may not work offline.
