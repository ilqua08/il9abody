# il9aBody

A dark, English-language workout and nutrition progressive web app. It keeps the user's workout history, food log, goals, plan, XP and reminders in browser local storage on the current device.

## Preview locally

Serve this folder through a local HTTP server and open its address in a browser. The service worker and PWA installation require HTTPS (or localhost); opening `index.html` directly from Files does not enable them.

## Install on iPhone

1. Publish this folder at an HTTPS URL using a static host.
2. Open that URL in **Safari** on the iPhone.
3. Tap **Share → Add to Home Screen → Add**.
4. Launch il9aBody from its new Home Screen icon.

The app shell is cached for offline use after the first successful load. Data is local to that browser installation and is not synchronized. Use **Profile → Export backup** before clearing browser data or changing devices.

## Notifications

Workout and nutrition reminder times are checked while the app is open. iOS does not provide reliable background scheduled notifications to this static PWA. Web push needs an installed app, user permission, a push subscription service and a server; none is included here. The timer can also alert while the app is open; a foreground browser notification is attempted when permission has been granted.

## Deploying

Upload the complete folder without changing its relative paths. No build step or external runtime dependency is required. A static HTTPS host is still needed for sharing/installing the app; this project has not been hosted or published to the App Store.
