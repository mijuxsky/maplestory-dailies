# MapleStory Dailies

A minimal tracker for your dailies in MapleStory.

## Features

- **Themes** — Light, Cloud (Light), Lavender (Light), Matcha (Light), Dark, Evergreen (Dark). Theme control sits under the UTC clock.
- **UTC clock** — Shows current UTC time in `MM/DD/YYYY HH:MM:SS`. Dailies reset at **00:00 UTC**.
- **Presets** — 3 local Presets (1–3). Switch presets to load a different set of characters/tasks.
- **Save / Load** — Minimal **Save (💾)** and **Load (📂)** icons next to *Preset* export/import your data as JSON. No servers used.
- **Add character** — “+ Add Character” on the far right. Max 20 characters. Starts with 2 tasks (min 1, max 10).
- **Zero cards** — You can keep zero character cards (no minimum required).
- **Keyboard** — Enter/Tab/↓ inserts a new task under the current one; ↑/Shift+Tab goes up; ←/→ switches cards.
- **Reorder cards** — Drag and drop or use the small ↑/↓ arrow buttons on each card. Smooth slide animation. Drops are limited to the existing number of slots.
- **Reorder tasks** — Drag a task by the ⋮⋮ handle within its card to change priority.
- **Insert task** — With a task focused, press **Enter** to insert a task directly beneath it.
- **Check All** — A master checkbox at the **bottom** of each card toggles all task checkboxes.
- **Upload avatar** — Use the camera/upload icon on a card to set a custom image (replaces “Set Avatar”).
- **MapleRanks lookup** — Typing a name in “Character Name” and confirming (Enter or blur) fetches avatar, level, and class via your configured proxy.
- **Delete confirm** — Deleting a card prompts: *“Are you sure you want to delete the character: &lt;Name&gt;?”* with **Yes/No** buttons (monochrome, minimal).
- **Popup notice** — If a popup blocker prevents opening the confirm dialog, an inline alert asks you to allow popups for the site.
- **Import/Export** — Move data between devices with the Save/Load JSON file.

## How to Use

- **Theme & preset** — Pick a *Theme* under the UTC clock; choose a *Preset* (1–3) to switch data sets.
- **Save/Load** — Click **💾 Save** to download JSON. Click **📂 Load** to import a JSON file.
- **Add characters** — Press **+ Add Character** (top right). Edit *Character Name* and tasks inline.
- **Keyboard** — Use **Enter/Tab/↓** to jump to next task and insert below; **↑/Shift+Tab** to go up; **←/→** to switch cards.
- **Reorder cards** — Drag a card or click the card’s **↑/↓** controls to move it. Slots limited to current count.
- **Reorder tasks** — Grab the **⋮⋮** handle to move a task within a card.
- **Check All** — Use the **Check All** box at the bottom of the card to toggle all tasks.
- **Upload avatar** — Click the card’s upload icon to add a custom image. (Character Name can also auto-fetch from MapleRanks.)
- **Delete** — Click **×** and confirm in the dialog. If blocked, allow popups and retry.
- **Reset** — Checkboxes reset automatically at **00:00 UTC**.

---

**Local storage:** All data is saved in your browser per preset. Switching devices? Use **Save/Load** to transfer JSON.
