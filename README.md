# Couchfront — website

Public marketing site for **Couchfront**, the Windows launcher that brings your PC game library to the couch: it syncs games from Steam, Epic, GOG, Xbox, EA, Ubisoft, Amazon, Battle.net and itch.io into Steam with artwork, so everything browses and launches from the couch with a controller.

- Site: https://kiyiyip.github.io/couchfront/
- Download (portable .exe): https://kiyiyip.github.io/couchfront/downloads/Couchfront-Portable.exe

## What lives here

Only the published site: the four static pages, styles, screenshots, the browser demo (`demo/`), and the latest portable build (`downloads/`). The application source stays in a private repository.

## Publishing

Run from a checkout of the private repository:

```sh
npm run build:exe     # builds src-tauri/target/release/couchfront.exe
npm run publish:site  # mirrors website/ here, drops in the exe, commits, pushes
```

GitHub Pages serves this repository's `main` branch root directly (Settings → Pages → Deploy from a branch) — no workflow needed.
