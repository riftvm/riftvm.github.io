# RiftVM website

Static GitHub Pages website for RiftVM: Omarchy and macOS workspaces on Apple silicon Macs running **macOS 27 or later**.

The maintained page and styles live in `riftvm/riftvm` under `docs/index.html` and `docs/styles.css`. This repository contains the publishing copy: copy the page, rename `styles.css` to `style.css` and update its stylesheet link, and copy referenced assets into `assets/` when updating it. Keep `catalog/` intact.

Guide visitors to Homebrew installation or GitHub Releases. Do not hardcode an app release version or describe the app as awaiting release. Keep the host requirements visible beside installation instructions.

Preview with `python3 -m http.server 8765`, then open `http://localhost:8765`.

No build dependencies, analytics, remote fonts, or third-party scripts.
