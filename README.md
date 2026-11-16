# stqv-assets — QC Station home-screen launcher (STQV-LNC-001)

Public files only: icons + a tiny launcher page. **No production data, no secrets.**
The launcher gives tablets a real home-screen icon (Chrome needs a web manifest, which Apps Script cannot serve)
and immediately opens the Apps Script web app **Station Tablet QC Visual** (`/exec?device=TAB-xx`) — no frame,
so the Minebea Google sign-in works normally.

- Install: in the app, เพิ่มเติม → **ไอคอนหน้าจอ** (opens `…/stqv-assets/?install=1&device=TAB-xx`) → ติดตั้ง.
- Daily use: tap the **QC Station** icon → redirected to the Apps Script link.
- `index.html` → `EXEC` = production deployment `/exec`. Change it if the deployment id changes.

| Rev | Date | Who | Change |
|---|---|---|---|
| A | 2026-11-16 | Thanongsak (with Claude) | Redirect launcher (replaces the withdrawn iframe PWA): manifest + microscope icons (any + maskable), install screen with beforeinstallprompt / manual steps, device remembered |
