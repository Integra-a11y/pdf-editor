# PDF Editor

PDF reader and editor that runs entirely in the browser: word-level text editing, real deletion, shapes, images and layers, forms, signatures, OCR, Swiss QR-bill and invoicing with a client base. Interface in French, German, English, Italian and Russian.

## Install

Open the published page in Edge or Chrome, then use **Install** (address bar icon, or Settings > Install the app). The app gets its own window and Start menu icon, works offline and appears in "Open with" for PDF files.

## Repository layout

- `web/` the app, served as is (no build step)
- `tools/build-sw.mjs` regenerates `web/sw.js`, the offline cache list, from the files in `web/`
- `.github/workflows/pages.yml` publishes `web/` to GitHub Pages on every push to `main`

## Data

Documents never leave the computer. Invoicing data (clients, invoices, settings) is stored in the browser profile of each computer: export clients to CSV for backups.

## Licence

GNU AGPL v3.0 (see `LICENSE`), because the app includes MuPDF. Third-party components and their licences are listed in `THIRD-PARTY-NOTICES.txt`.
