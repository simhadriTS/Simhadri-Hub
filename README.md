# NTPC Simhadri Plant Hub (single-file build)

`index.html` contains everything: opening screen, Plant Guide, Area Owner Finder, logo and data.
It works from GitHub Pages, an intranet server, or opened directly as a file.

## GitHub Pages (repo: Simhadri-Plant-Hub)
Required:  index.html
Recommended (upload with folders kept):
- data/locations.json, data/land.json  : live Plant Guide data; target of the Plant Guide "Publish to GitHub" admin function
- manifest.webmanifest, service-worker.js, icons/, favicon.ico : "Install app" / Add to Home screen and offline use
- 404.html, .nojekyll
Delete the old guide/ and owner/ folders if you uploaded them earlier.

## Admin
- Plant Guide: 🔒 Admin login (top right); GitHub token via Admin → section 4.
  The token must have Contents: Read and write on THIS repo (Simhadri-Plant-Hub).
- Area Owner Finder: 🔒 Admin (top right); password in index.html (search ADMIN_PASSWORD).

## Updating
After any code change, bump CACHE in service-worker.js (plant-hub-v2 -> v3).
