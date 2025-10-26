# Collapsible Sections + iOS Safe-Area + Icon
- Title now respects iOS safe-area (no overlap with the time).
- Each section (**Today**, **This Week**, **Future**) is **collapsible**. Default state is collapsed; tap header to expand.
- Per-section counters (done/total) are shown beside the title.
- Delete button visual glitch fixed on iOS (removed stray white mark).
- Mobile drag still supports auto-scroll and precise drop position.
- `icons/logo.png` is used for iOS Home Screen and manifest.

## Tips
- Collapsed state is saved in localStorage (`task-tracker:collapsed`).
- If the iOS icon doesn’t refresh, rename the PNG and update paths in `index.html` & `manifest.webmanifest` to bust cache.
