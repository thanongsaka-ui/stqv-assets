# stqv-assets — QC Station PWA wrapper (STQV-PWA-001)

Public files only: icons + a small PWA shell that frames the Apps Script web app
**Station Tablet QC Visual**. No production data, no secrets.

- App URL: https://thanongsaka-ui.github.io/stqv-assets/  (add `?device=TAB-03` once per tablet; it is remembered)
- Install on tablet: open the URL in Chrome → ⋮ → **Install app** / Add to Home screen.
- If Google sign-in cannot run inside the frame, the splash shows **เปิดระบบ** which opens the app directly.
- `index.html` → `EXEC` = production deployment `/exec` URL. Change it when the deployment id changes.
- `sw.js` caches only the shell; bump `VER` when shell files change.

| Rev | Date | Who | Change |
|---|---|---|---|
| A | 2026-11-16 | Thanongsak (with Claude) | First PWA wrapper: manifest (fullscreen, yellow theme), microscope icons incl. maskable, service worker (shell only), ready-handshake + direct-open fallback |
