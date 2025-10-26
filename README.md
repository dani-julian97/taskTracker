# Safari Home Screen Icon Setup

This package updates your app so **iOS Safari uses `icons/logo.png`** as the Home Screen icon.

## What’s included
- `index.html`: adds the right `<link rel="apple-touch-icon">` and PWA meta tags.
- `manifest.webmanifest`: points to `icons/logo.png` for installable icon (Chrome/Android and iOS 17+).
- `icons/` (empty placeholder): put your **existing** `icons/logo.png` here.

## Requirements for the icon
- Recommended: **180×180 PNG** (works great on iPhone). Larger (e.g. 1024×1024) is okay too; iOS downsizes.
- Avoid transparency for best results. Keep safe margins (no content too close to edges).

## How to use
1. Copy your current `icons/logo.png` into this folder at `icons/logo.png` (replace if prompted).
2. Open `index.html` (or deploy). On iPhone:
   - Safari → Share → **Add to Home Screen**.
   - The shortcut should show your icon.
3. If the old icon is cached, try:
   - Rename the file once (e.g., `logo-v2.png`) and update both `index.html` and `manifest.webmanifest` to match.
   - Or clear Safari Website Data: *Settings → Safari → Advanced → Website Data → Remove All Website Data*.

## Notes
- We set `apple-mobile-web-app-capable=yes` so it runs full-screen as a web app.
- `theme-color` and status bar are tuned for your dark theme.
