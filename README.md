### Auto-fill (Maple Ranks)
- **What**: When you type a Character Name, the app calls a Cloudflare Worker that fetches your Maple Ranks profile and extracts **Level**, **Job**, and **Avatar**.
- **When images change**: If you have **not** uploaded a custom avatar, the fetched avatar is applied automatically. If you **have** uploaded an avatar, the auto-image will **not** replace it.
- **Storage**: Avatar URLs and the “user uploaded” flag are saved in your preset data. Save/Load includes both.

### Quick tests
- **Image fetch**: Type a known character name, pause ~0.5s → Level/Job appear; avatar shows automatically if no user image.
- **Precedence**: Upload an avatar, then change the name → Level/Job update but your uploaded image remains.
- **Save/Load**: Save JSON, refresh page, Load the same file → characters, tasks, Level/Job, and avatar all restore.
- **Errors**: Type a random name → brief “Not found” message; existing fields unchanged; no console errors.
