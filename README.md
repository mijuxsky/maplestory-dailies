# MapleStory Dailies

A minimal tracker for your dailies in MapleStory.

## Features

- **Themes**: Light, Cloud (Light), Lavender (Light), Matcha (Light), Dark, Evergreen (Dark). Theme control sits under the UTC clock.
- **UTC clock**: Shows current UTC time in `MM/DD/YYYY HH:MM:SS`. Dailies reset at 00:00 UTC.
- **Presets**: Three local presets (1-3). Switch presets to load a different set of characters and tasks.
- **Save and Load**: Minimal Save (💾) and Load (📂) icons next to Preset export or import your data as JSON. No servers used.
- **Add character**: “+ Add Character” on the far right. Up to 20 characters. Starts with two tasks (minimum 1, maximum 10).
- **Zero cards**: You can keep zero character cards.
- **Keyboard**: Enter, Tab, and Down insert a new task under the current one. Up and Shift+Tab go up. Left and Right switch cards.
- **Reorder cards**: Drag and drop with smooth animation or use the small Up and Down arrow buttons on each card. Sorting uses SortableJS.
- **Reorder tasks**: Drag a task by the ⋮⋮ handle within its card to change priority.
- **Insert task**: With a task focused, press Enter to insert a task directly beneath it.
- **Check All**: A master checkbox at the bottom of each card toggles all task checkboxes.
- **Upload avatar**: Use the upload icon on a card to set a custom image.
- **MapleRanks lookup**: Typing a name in “Character Name” and confirming (Enter or blur) fetches avatar, level, and class through your proxy.
- **Delete confirm**: Deleting a card prompts “Are you sure you want to delete the character: <Name>?” with Yes and No buttons. Monochrome and minimal.
- **Popup notice**: If a popup blocker prevents the confirm dialog, an inline alert asks you to allow popups for the site.
- **Import and Export**: Move data between devices with the Save and Load JSON file.

## How to Use

- **Theme and preset**: Pick a Theme under the UTC clock. Choose a Preset (1-3) to switch data sets.
- **Save and Load**: Click 💾 Save to download JSON. Click 📂 Load to import a JSON file.
- **Add characters**: Press + Add Character. Edit Character Name and tasks inline.
- **Keyboard**: Use Enter, Tab, or Down to jump to the next task and insert below. Use Up or Shift+Tab to go up. Use Left or Right to switch cards.
- **Reorder cards**: Drag a card or click the card’s Up or Down controls to move it. Cards drop into the grid slots.
- **Reorder tasks**: Grab the ⋮⋮ handle to move a task within a card.
- **Check All**: Use the Check All box at the bottom of the card to toggle all tasks.
- **Upload avatar**: Click the card’s upload icon to add a custom image. Character Name can also auto fetch from MapleRanks.
- **Delete**: Click × and confirm in the dialog. If blocked, allow popups and retry.
- **Reset**: Checkboxes reset automatically at 00:00 UTC.

---

**Local storage**: All data is saved in your browser per preset. Switching devices? Use Save and Load to transfer JSON.
