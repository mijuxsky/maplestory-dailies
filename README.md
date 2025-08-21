# MapleStory Dailies

A minimal tracker for your dailies in MapleStory.

## Features
- Manage up to **20 characters**, each with a name and checklist
- **Duplicate** or **Delete** a character card from its top toolbar
- **Drag & drop** cards to reorder (snap-to-grid layout)
- Tasks per character: **min 1**, **max 10**; start with **2** lines by default
- **Keyboard navigation**:
  - **Enter / Tab / ↓** → go to next task (auto-adds a new line at the end)
  - **↑ / Shift+Tab** → previous task (jumps to name if above first)
  - **← / →** at field edges → move to previous/next character card
- **Presets** dropdown to switch between three saved configurations (stored locally in your browser)
- **Auto-reset** of checkboxes at **00:00 UTC** daily
- **UTC clock** at the top in **MM/DD/YYYY** format
- **Instructions panel** with **Hide/Unhide** toggle
- **Themes**:
  - Light: **Light Mode**, **Cloud (Light)**, **Lavender (Light)**, **Matcha (Light)**
  - Dark: **Dark Mode**, **Evergreen (Dark)**
  - Transparent, theme-matching dropdown menus and legible contrast in dark modes
- **Character images**:
  - Per-card **Region** and **World** selectors and a minimal **Fetch** button
  - Uses Nexon rankings via a **Cloudflare Worker** proxy
