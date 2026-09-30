# RiftVM website

Static GitHub Pages website for RiftVM: Omarchy Linux, full screen and GPU-accelerated, on Apple silicon Macs running **macOS 27 or later**.

This repository is the canonical source of the website: edit `index.html`, `style.css`, `copy-command.css`, `copy-command.js` and `assets/` here. The copy that used to be maintained in `riftvm/riftvm` under `docs/` is being removed, so nothing is synced from there any more.

Stylesheets and scripts are linked with an `?asset=` query holding the first 12 hex characters of the file's SHA-256. After changing one of those files, update its query in `index.html` and run `bin/check-asset-hashes`; the deploy workflow runs the same check and refuses to publish a page whose hashes or local references do not match.

`catalog/linux.json` is served for legacy RiftVM clients (0.4 and earlier), which still download it from this site, so it must be kept.

Guide visitors to Homebrew installation or GitHub Releases. Do not hardcode an app release version or describe the app as awaiting release. Keep the host requirements visible beside installation instructions.

Preview with `python3 -m http.server 8765`, then open `http://localhost:8765`.

No build dependencies, analytics, remote fonts, or third-party scripts.
