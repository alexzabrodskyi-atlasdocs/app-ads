# app-ads.txt for atlasdocs.app

Public app-ads.txt served via GitHub Pages at
https://ads.atlasdocs.app/app-ads.txt.

`https://atlasdocs.app/app-ads.txt` 301-redirects here so the file
renders inline in browsers instead of triggering a download (Squarespace's
File Manager forces `Content-Disposition: attachment`).

## Source of truth

This repo. `app-ads.txt` on `main` is what GitHub Pages publishes; it
re-deploys 1-2 minutes after a push. There is no other copy to sync.

## Editing

- Keep each network's block whole, as the network supplied it. Refresh a
  block by replacing it with the network's current list. Lines that repeat
  across blocks are intentional; do not deduplicate them.
- Every AdMob mediation adapter in `atlas_pro/atlasapp/Podfile` needs its
  network's DIRECT line here. Adding or removing an adapter means editing
  this file too.
- Save as UTF-8 without BOM, LF line endings.
