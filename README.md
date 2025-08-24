# MapleStory Dailies

A single‑file, theme‑aware, keyboard‑friendly daily checklist for MapleStory characters. Everything lives in `index.html`—no build step required.

## Quick start
1. Download or clone this project.
2. Open **index.html** in any modern browser (Chrome, Edge, Firefox, Safari).
3. Pick a theme, add characters, and start tracking tasks.
4. Use **Save** to export your data (JSON) and **Load** to import it later.

> **Storage:** All changes are saved to your browser’s `localStorage` per preset. No backend.

## Features
- **Character cards**
  - Avatar (auto‑lookup or manual upload), Level/Class, centered **Character Name** line.
  - Up to 10 tasks per character; drag to reorder.
  - Task priorities: **normal / important / urgent** with subtle, theme‑aware highlighting.
  - **Check All** per card.
- **View chips** (centered below the name)
  - **Show priority first** – groups urgent/important to the top (default).
  - **Only priority** – hides normal tasks.
- **Presets (rename‑only)**
  - Exactly **three presets (1–3)** with stable IDs.
  - Rename the current preset via the small **pencil** next to the Preset dropdown.
  - Validation: **required**, **unique** among the three, **max 12 chars**, trims spaces.
  - Names persist; IDs never change.
- **Theming**
  - Light: **Light Mode, Cloud, Lavender, Matcha, Milk Tea**  
  - Dark: **Dark Mode, Nightshade (Dark Purple), Evergreen, Midnight Blue, Mocha**
  - All controls use shared tokens for colors, borders, shadows, and focus rings.
- **Contact & Support**
  - Top‑right **Contact** button with a tiny **envelope + small heart** icon (cute, minimal).
  - Modal (focus‑trapped, Esc/backdrop to close) with:
    - **Ko‑fi:** `https://ko-fi.com/mijuxsky` (opens in new tab)
    - **Discord:** `MijuxSky` + **Copy** button and brief toast (“Discord handle copied”).
  - Icons are monochrome and inherit the current theme color.
- **Accessibility**
  - Keyboard focus rings on interactive controls.
  - Modal has `role="dialog"`, `aria-modal="true"`, returns focus to opener.
  - Screen reader announcements for preset rename and validation errors.
  - Subtle status messages when priorities change or lookups run.
- **Import/Export**
  - Export saves `{version, preset, characters}` JSON.
  - Import restores characters/tasks (up to the app’s limits).

## Keyboard shortcuts
> Open **?** (top‑right) to see these in‑app.
- **Up/Down** – Move between tasks
- **Enter** – Insert a new task below the focused task
- **Tab** – Toggle the focused task’s checkbox
- **Space** – Toggle a row when the checkbox or row is focused
- **Alt + A** – Open **Accents** panel for the focused text input
- **Esc** – Close panels/modals

## Data & persistence (overview)
- Theme: `mapleTheme`
- Current preset: `maplePreset`
- Preset names: `maplePresetNames_v1` (object with keys `1`,`2`,`3`)
- Per‑preset data: `mapleData_v2_preset{N}` stores character/task state
- Daily checkbox state: stored separately per date/preset/character/task (keys derived like `check_YYYY-MM-DD_preset{N}_c{i}_t{t}`)

> Tip: To “reset” the day, you can clear today’s `check_…` keys from DevTools > Application > Local Storage.

## Customization
- **Themes:** Adjust CSS variables in `:root` and theme body classes.
- **Contact modal:** Update the Ko‑fi URL or Discord handle in the modal markup.
- **Icons:** Inline SVGs inherit `currentColor`; swap paths to change pictograms.
- **Accents:** The small accents helper can be extended in `renderAccents()`.

## Troubleshooting
- **No layout shift, but a control looks off in one theme** – check theme tokens for border/background contrast.
- **Discord icon looks clipped** – the modal uses `overflow:visible` on the icon SVG and a small internal transform to avoid clipping; clear cache if you still see it.
- **Auto‑lookup is slow** – results are cached; give it a moment, or enter at least 4 characters before hitting Enter to force a lookup.

## What changed recently
- Centered the **Character Name** row with a left spacer to mirror the Accents button.
- **Centered** the “Show priority first” and “Only priority” chips.
- **Contact** button now uses a **tiny envelope with a small heart** icon.
- Contact modal redesigned to a **minimal** layout with **full Ko‑fi link** and **Discord** + **Copy** (toast).
- Fixed a **Discord icon** clipping issue inside the modal.
- Preset **Rename** added (pencil icon): required, unique, **12‑char** limit; IDs stay the same.
- Small JS fixes (e.g., invalid object literal initializer) to resolve console errors.

## Tech notes
- Pure client‑side HTML/CSS/JS; uses **SortableJS** (CDN) for drag‑and‑drop.
- Fonts: Google Fonts **Quicksand**.
- No build tools, no framework—open `index.html` directly.

## License
Add your preferred license here (e.g., MIT).

---

**Contact**  
Ko‑fi: https://ko-fi.com/mijuxsky  
Discord: MijuxSky
