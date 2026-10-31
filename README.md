# Cosmic Cards updates

This repository hosts the update files for the **Cosmic Cards** Windows app. It holds no source code.

- `latest.json` describes the newest game version. It's signed, and the app rejects anything not signed with the developer's key.
- `game-<version>.html` is the game itself. The app checks its SHA-256 against `latest.json` before using it.

Installed copies check `https://raw.githubusercontent.com/lee34674/cosmic-cards-updates/main/latest.json` each time they start, and every few hours while running.
