# MapleStory Dailies

A minimal tracker for your dailies in MapleStory.

## Key Features
- **Themes & Presets** — Light (Light, Cloud, Lavender, Matcha) and Dark (Dark, Evergreen). Three local **Presets** to save/load layouts.
- **Characters & Tasks** — Up to 20 characters. Each starts with 2 tasks (min 1, max 10). Everything saves locally in your browser.
- **Keyboard** — Enter/Tab/↓ to move forward (auto-adds lines); ↑/Shift+Tab up; ←/→ to switch cards at edges.
- **Reorder cards** — Drag any character card to any position in the grid.
- **Reorder tasks** — Drag the **⋮⋮** handle to change task priority within a card.
- **Insert between** — Press **Enter** on a task to insert a new line directly **below** it.
- **Check-All per card** — A “Check All” toggle above tasks marks/unmarks all checkboxes. Shows an indeterminate state when mixed.
- **Avatars & Info** — From the card’s name field or **Set Avatar** popup, fetch avatar + **Lv./Class** from MapleRanks (via your Worker). Or upload an image.
- **Daily reset** — All checkboxes reset automatically at **00:00 UTC**. Live UTC clock shown in **MM/DD/YYYY** format.
- **Import/Export** — Save your data to a JSON file and restore it on another device (no servers).
- **Delete confirm** — Deleting a character asks: **“Are you sure you want to delete the character: &lt;Character Name&gt;?”** (Yes/No).

## How to Use
1. **Themes & Presets** — Pick a Theme and one of 3 Presets (stored locally).
2. **Add Characters** — Click **+ Add Character** (max 20).
3. **Set Avatar** — Camera → *Set Avatar* (or type the name in the card and press **Enter**).
4. **Enter Tasks** — Type and press **Enter** to add a line; use **Tab/Arrows** to navigate.
5. **Reorder** — Drag cards anywhere; drag **⋮⋮** to reorder tasks.
6. **Check All** — Toggle the card’s **Check All** to mark/unmark all tasks at once.
7. **Backup** — **Export** to JSON; **Import** to restore on another device.

## Notes
- The Worker endpoint used for MapleRanks lookups is configured in `index.html` as `PROXY_URL`.
