# Block Select

A single-page Minecraft launcher for an offline game library. It lets you browse a collection of HTML-based Minecraft versions and clients, open them in a viewer, and use a mobile-friendly overlay with touch controls.

## Features

- Clean dark-themed launcher UI
- Auto-discovers game HTML files in the same folder when supported by the browser
- Built-in list of included versions and clients
- Search and category filters
- Safe local play via a browser-based viewer iframe
- Mobile controls for movement, actions, and camera look
- Top toolbar buttons for Menu, Chat, View, and Layout editing
- Control editor with drag, resize, color, and picture customization
- Saves per-game layout preferences locally in the browser

## Run locally

From this folder, serve it with a local web server:

```bash
cd /workspaces/eaglercraft-versions
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Notes

- This project is intended for local use and offline HTML game files.
- Some browsers may restrict folder access or pointer lock behavior. The launcher includes fallbacks for compatibility when possible.
- Mobile controls and layout edits are injected into the game page at runtime for same-origin local pages.

## Included games

The launcher ships with a starter library that includes many of the HTML versions and clients in this folder, including classic builds and several newer variants.

## Files

- `index.html` — main launcher UI and mobile overlay logic
- game HTML files — the Minecraft builds and clients to open from the launcher

## Important

This repository does not include a Minecraft server or any copyrighted game assets beyond the local HTML files in the workspace. It is a launcher and client browser wrapper for locally stored game builds.
