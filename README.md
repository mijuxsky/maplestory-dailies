# MapleStory Dailies

A minimal tracker for your dailies in MapleStory. Runs fully in the browser and stores data locally per preset.

---

## Features

- **UTC clock**  
  Shows current UTC time in `MM/DD/YYYY HH:MM:SS`.

- **Daily reset**  
  Task completion is keyed by UTC date so checkmarks reset each day automatically.

- **Themes**  
  Light themes first, then dark. All UI elements follow tokens for backgrounds, text, borders, focus rings, buttons, dialogs, tooltips, and panels.  
  Light: Cloud, Lavender, Light Mode, Matcha, Milk Tea  
  Dark: Dark Mode, Evergreen, Midnight Blue, Mocha, Nightshade

- **Presets**  
  Three starter presets selectable from the toolbar. All data is saved per preset.

- **Save and Load**  
  Save exports a JSON file. Load imports a JSON file. Works offline and keeps data per preset.

- **Characters**  
  Add, duplicate, delete with confirmation. Drag and drop cards to reorder. Use Up and Down arrows on each card as an alternative.

- **Accents**  
  Per card Accents button next to Character Name. Insert accented letters without losing focus. Alt + A opens accents for the focused field.

- **Maple Ranks lookup**  
  Type a Character Name and the app looks up Job and Level via the Worker proxy. If available and no uploaded avatar exists, the image is set automatically. If no match is found the Job shows “Character not found on MapleRanks” in a soft red. Level and image are not changed.

- **Avatars**  
  Upload a custom character image. User uploads are never overwritten by auto lookups.

- **Tasks**  
  Each card starts with two lines. Enter inserts a new task below the current line. Tab toggles the checkbox on the focused row. Up and Down move between rows.

- **Priority**  
  Click the small Priority button on a row to cycle Normal, Important, Urgent. Important uses the theme accent. Urgent uses the theme soft red and a brief glow on the left bar. Chips above the list let you show priority first or only priority. P is not used as a shortcut to avoid interrupting typing.

- **Reorder tasks**  
  Drag by the vertical handle at the end of the row. Reordering stays within the card and preserves state.

- **Check All**  
  A Check All control at the bottom of each card toggles all tasks in that card. The label uses a theme muted color distinct from task text.

- **Keyboard shortcuts**  
  A “?” button opens a centered modal with keyboard help and a Quickstart. Press “?” globally to open. Esc closes. Focus returns to the opener.

---

## Quickstart

1) **Choose preset**  
   Use Preset on the toolbar.

2) **Enter name**  
   Type Character Name. Use Accents if needed.

3) **Wait or upload**  
   After a short pause Job and Level update. Upload an avatar if you prefer.

4) **Review tasks**  
   Check items and set priorities if useful.

5) **Save**  
   Click Save to export a backup JSON.

6) **Load or manage**  
   Load another preset file or switch presets.

---

## Keyboard

- **Open help**  
  Click “?” or press “?” to open the Shortcuts modal. Esc closes.

- **Move between tasks**  
  Up and Down arrows.

- **Toggle a task**  
  Space or Tab on the focused row.

- **Insert below**  
  Enter creates a new task directly under the current row.

- **Accents**  
  Alt + A opens Accents for the focused input.

Typing in task fields is never intercepted by global shortcuts.

---

## Data and storage

- **Local storage**  
  All data is stored in the browser per preset and per UTC day for checkmarks.

- **Export and import**  
  Save exports JSON. Load imports JSON. No servers are used.

- **Daily reset**  
  Checkmarks reset with the new UTC date. Task text and ordering persist.

---

## Maple Ranks lookup

- **Source**  
  Queries Maple Ranks through a Cloudflare Worker proxy.

- **Fields**  
  Updates Job and Level. If no user avatar exists and an image URL is returned, the avatar is set automatically.

- **On failure**  
  Job shows “Character not found on MapleRanks” in a soft red. Level and image are unchanged.

- **Uploads win**  
  User uploaded avatars are never overwritten by lookups.

---

## Tips

- **Reorder cards**  
  Drag a card by the invisible strip above the Character Image or use the Up and Down arrows on the card.

- **Reorder tasks**  
  Drag by the vertical handle on each row.

- **Insert quickly**  
  Press Enter on a task to insert a new one right below.

- **Check all**  
  Use the Check All control at the bottom of the card.

---

## Theming

All themes define tokens for background, panel, card, border, text, text weak, accent and tint, soft red, focus ring, and tooltip or dialog surfaces. The app applies these tokens to cards, buttons, inputs, selects, icons, dialogs, tooltips, accents panel, and the Shortcuts modal. Focus rings meet contrast guidelines.

---

## Troubleshooting

- **UTC shows dashes**  
  Wait a moment or refresh. The clock updates once per second.

- **No image after typing a name**  
  Either Maple Ranks had no avatar or the Worker returned no image. Upload your own or try again later.

- **Import fails**  
  Make sure you load a JSON file exported by the app.

- **Nothing saves**  
  Check that your browser allows local storage.

---

#
