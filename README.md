# RiftVM website

Official website: <https://riftvm.com/>. <https://riftvm.github.io/> also reaches
this site through GitHub Pages' custom-domain redirect.

The application source and downloads remain in
[`riftvm/riftvm`](https://github.com/riftvm/riftvm).

## Publish

Edit this repository's HTML, CSS, scripts, images and public Linux catalog.
Run `./bin/check-asset-hashes` before committing. Pushes to `main` run
`.github/workflows/pages.yml` and publish the static site through GitHub Pages.
`riftvm.com` is the existing custom domain; retain its configuration.

Preview with `python3 -m http.server 4186` and open <http://localhost:4186/>.
Support is published at `/support/`.
