# MapleStory Dailies

A minimal tracker for your dailies in MapleStory.

## Features

- **Themes**: Choose from Light, Cloud (Light), Lavender (Light), Matcha (Light), Dark, and Evergreen (Dark). Theme is saved locally.
- **UTC clock**: Live UTC time in `MM/DD/YYYY HH:MM:SS` format.
- **Presets**: Three independent presets (1–3). Each stores its own characters, tasks, and theme.
- **Save / Load**: Export your data to a JSON file and import it later — no servers required.
- **Characters**: Up to 20 character cards. Cards start with 2 tasks (minimum 1, maximum 10).
- **Add / Duplicate / Delete**: Add new cards, duplicate existing ones, or delete with confirmation.
- **Delete prompt**: “Delete the character: \<Character Name\>?” with **Yes** then **No**.
- **Upload avatar**: Set a custom image per character from your device.
- **Tasks**: Up to 10 tasks per character. Enter/Tab inserts a task under the current one.
- **Reorder tasks**: Drag by the ⋮⋮ handle; checkbox state is preserved.
- **Reorder cards**: Drag from the invisible strip above the name or use the Up/Down arrows. Smooth animation.
- **Check All**: Bold “Check All” line at the bottom of each card toggles all tasks for that card.
- **Daily reset**: All task checkboxes reset automatically at 00:00 UTC.
- **Local-only**: Everything runs entirely in your browser with `localStorage`. No accounts or servers.

## How to Use

- **Pick theme**: Use the Theme dropdown at the top-left.
- **Choose preset**: Under the How to Use box, select Preset 1–3.
- **Save / Load**: Use the 💾 Save to export JSON; 📂 Load to import JSON.
- **Add character**: Click **+ Add Character** (left side of the toolbar).
- **Type name**: Click the name line to edit your character’s name.
- **Upload avatar**: Click the upload icon on a card to set an image.
- **Add tasks**: Press Enter or Tab in a task line to insert another below it.
- **Reorder tasks**: Drag the ⋮⋮ handle to rearrange; state is preserved.
- **Reorder cards**: Drag from the invisible strip above the name, or use the Up/Down arrows.
- **Check All**: Use the bold “Check All” at the bottom of a card to toggle all tasks.
- **Delete card**: Click × then confirm “Yes” in the prompt.

### Auto-fill (Maple Ranks)
- **What**: When you type a Character Name, the app calls a Cloudflare Worker that fetches your Maple Ranks profile and extracts **Level**, **Job**, and **Avatar**.
- **When images change**: If you have **not** uploaded a custom avatar, the fetched avatar is applied automatically. If you **have** uploaded an avatar, the auto-image will **not** replace it.
- **Storage**: Avatar URLs and the “user uploaded” flag are saved in your preset data. Save/Load includes both.

### Quick tests
- **Image fetch**: Type a known character name, pause ~0.5s → Level/Job appear; avatar shows automatically if no user image.
- **Precedence**: Upload an avatar, then change the name → Level/Job update but your uploaded image remains.
- **Save/Load**: Save JSON, refresh page, Load the same file → characters, tasks, Level/Job, and avatar all restore.
- **Errors**: Type a random name → brief “Not found” message; existing fields unchanged; no console errors.
