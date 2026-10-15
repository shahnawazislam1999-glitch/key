# PhoneDeck PWA (launcher)

Installable, fullscreen, works offline. Paste the PC link (`http://192.168.x.x:8080/?key=...`), tap Connect.

## Host on GitHub Pages
1. Create a repo, upload the *contents* of this folder (index.html, sw.js, manifest.webmanifest, icons/) to the repo root.
2. Settings > Pages > Deploy from branch > `main` / root.
3. Open `https://<you>.github.io/<repo>/` on the phone (Chrome) once, online.
4. Chrome menu > **Install app** / **Add to Home screen**. After that it opens offline from the icon.

## Notes
- The PWA is only the launcher. The keyboard/touchpad UI is served by the PC (phone.html), because browsers block
  an https page from talking to an http:// LAN server. Connecting just opens the PC page.
- Changing files later? Bump `VERSION` in sw.js so phones update.
