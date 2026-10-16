# P1K Desktop App Releases

This repository hosts **compiled installers only** for P1K's internal desktop apps:

- **P1K Portal** — admin dashboard
- **Synergyze Portal** — client management
- **Nivsh Media Admin** — Nivsh Media's admin panel

There is no source code here. Each app is a thin [Tauri](https://tauri.app) webview wrapper around a page already served at `p1k-ltd.com` — the actual application logic lives in P1K's private source repository. This repo exists solely so the installed apps can check for and download updates automatically (GitHub Releases require public access to be reachable by an unauthenticated client, which is why these live in a separate repo from the private source).

Releases are published automatically by CI on every push to the source repo that touches `desktop-apps/**`. Not intended for manual download by anyone outside P1K.
