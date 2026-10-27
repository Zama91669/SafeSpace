RIGHT NOW — MOBILE-READY PWA PACKAGE

Files:
- index.html: mobile-responsive Right Now app
- manifest.webmanifest: installable PWA metadata
- sw.js: basic app-shell caching for supported browsers
- icon.svg: app icon
- database.rules.json: deny-all Firebase Realtime Database rules

ANDROID APP
1. Install Node.js and Android Studio (with an Android SDK).
2. Run `npm install`.
3. Run `npx cap add android` once to create the native Android project.
4. Run `npm run cap:sync` to copy the current web app into the Android project and sync Capacitor.
5. Run `npm run cap:open` to open the project in Android Studio.

The web app files in the project root are the source files. Run `npm run cap:sync`
after changing them so the Android app receives the latest version. The app ID
is `com.rightnow.mobile`.

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
- This package does not itself deploy the app or publish Firebase security rules.
- `database.rules.json` denies all client reads and writes by default. To apply it, open Firebase Console > Realtime Database > Rules, replace the rules with the contents of this file, and publish. The app currently has no Firebase Authentication, so live database reads and SOS writes will be blocked while these rules are active. Do not enable public access to make the demo work; add authentication and user-scoped access rules first.
- This is a prototype and does not automatically contact emergency services. Do not rely on it as the only way to seek urgent help; call local emergency services directly when needed.
- The service worker caches the app shell, but external CDN libraries and Firebase real-time features may not work offline.
