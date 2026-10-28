A - LISTERS HUB (T & F SPRINTS COACH K) — INSTALLABLE PWA PROTOTYPE

FILES
- index.html: app interface
- app.js: navigation, coach editing, local persistence, search, swipe navigation
- programmes.json: extracted content from the six supplied Word documents
- manifest.webmanifest and sw.js: installability/offline caching
- icon.svg: app icon

IMPORTANT LIMITATIONS
1. This is a functional front-end prototype. It saves coach edits in the current browser/device only. It does NOT yet synchronize changes to athletes' separate phones.
2. To install as an app, host this folder on an HTTPS static host (for example, GitHub Pages, Netlify, or another HTTPS host). Opening index.html directly from disk is useful for previewing but will not enable full PWA installation/offline service-worker features.
3. The original training text is retained as text; Word tables are represented as pipe-separated rows. Check the display against the Word originals before using it for training delivery.
4. A basic local coach PIN is included, but it is not secure account authentication. No cloud database or live cross-device publishing is included. For secure coach-only editing and shared publishing, add server-enforced authentication and a shared database before public team use.

HOW TO USE
1. Open index.html in a browser for a local preview (programmes.json must stay beside it; local fetch may be blocked by some browsers, so HTTPS hosting is recommended).
2. Choose a phase, then a week, then a day. Swipe left/right in the session content or use Previous/Next.
3. Tap Coach login to edit, save, add sections, change branding, and export a JSON backup.
4. After hosting over HTTPS, open the site on a phone and choose Install app / Add to Home Screen from the browser menu.

See DEPLOYMENT_NEXT_STEPS.txt for the steps needed to enable hosting, secure roles, and shared publishing.
