# ✨ Palladium

> **A portal to play.** Palladium brings your favorite browser games together in one place.

[![Games](https://img.shields.io/badge/games-browser%20games-8b5cf6?style=for-the-badge)](./public/g.json)
[![Built with](https://img.shields.io/badge/built%20with-HTML%20%2B%20JavaScript-06b6d4?style=for-the-badge)](https://github.com/ItsTheif1/Palladium)

## 🎮 What is Palladium?

Palladium is a lightweight browser-games portal. Browse the catalog, pick a game, and jump straight in. Many game pages are served from this project; some launchers load game assets from the [UGS Assets collection](https://github.com/genizy/UGS-Assets), so an internet connection is required for those titles.

## 🕹️ Play

Open the deployed Palladium site and choose a title from the games page. The catalog is maintained in [`public/g.json`](./public/g.json). Each entry provides a display name, launch page, and icon.

### Recently added UGS titles

- 🪝 **Stickman Hook**
- 🐒 **Monkey Mart**
- 🐹 **Capybara Clicker**
- 🏈 **Football Bros**
- 🐷 **Iron Snout**

## 🧩 Add a game

1. Add a game launcher under `public/g/<game name>/index.html`.
2. Add an entry to the `games` array in `public/g.json`:

```json
{
  "name": "Game name",
  "filepath": "./g/Game name/index.html",
  "icon": "./g/Game name/icon.png"
}
```

Keep the JSON valid and use an icon path or image URL that is available to the browser.

## ⚠️ Notes

- UGS-hosted games and their icons are loaded from third-party CDN URLs and need internet access.
- Availability, embeds, and multiplayer features depend on those external services and may change independently of Palladium.
- Use the in-game controls shown by each title; some games work best on desktop.

## 💜 Credits

Palladium's portal is maintained in this repository. Game files and assets are credited to their respective creators and sources; UGS launchers reference [genizy/UGS-Assets](https://github.com/genizy/UGS-Assets).
