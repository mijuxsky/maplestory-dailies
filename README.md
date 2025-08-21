# MapleStory Dailies

A minimal tracker for your dailies in MapleStory.

## Features
- Pastel, light, dark, cloud, matcha, and evergreen themes (theme-aware controls and buttons).
- Three **Presets** saved locally (per browser) so different users can keep their own data.
- Add up to **20** characters; each starts with two checklist lines (min 1, max 10).
- **Keyboard flow:** Enter/Tab/↓ to next task (auto-adds a new line if needed); ↑/Shift+Tab up; ←/→ to move between cards.
- **Drag & drop** — place cards anywhere in the grid (row/column snap).
- **Character models & stats** pulled from **MapleRanks** via a proxy; or **Upload** your own (auto-resized to 150×110).
- Under the avatar, shows **“Lv. N Job”** when available (auto-updates after typing a name or using **Set Avatar**).
- **Set Avatar** popup: Set from MapleRanks, Upload, or Delete Avatar.
- **UTC clock** and daily reset at **00:00 UTC** for checkboxes.
- All data (including avatars, level/job text, and checkbox states) is stored in **localStorage**.

## How it works
- The site calls a Cloudflare Worker proxy with `?name=<CharacterName>` to fetch **avatar, level, and class/job** from MapleRanks.
- When you type a Character Name on a card, the Level & Job auto-update after a short pause. If no image is set yet, the avatar is filled too.
- Uploads are resized in-browser to 150×110 PNG using a canvas and saved locally.

## Hosting
- Designed for GitHub Pages (static `index.html`).