# ProtraxAR — Protractor Overlay PWA

A Progressive Web App that places a transparent, interactive protractor over any screen content. Designed for Chromebooks and Promethean boards.

---

## Setup Instructions

### Option A — Host it yourself (recommended for schools)

1. Copy all files to a web server or Google Cloud Storage bucket.
2. Ensure HTTPS is enabled (required for PWA install).
3. Share the URL with students/teachers.

### Option B — Use GitHub Pages (free & easy)

1. Create a GitHub account at github.com
2. Create a new repository named `protraxar`
3. Upload all files (index.html, manifest.json, sw.js, icons/)
4. Go to Settings → Pages → Source: main branch
5. Your app will be live at `https://yourusername.github.io/protraxar`

---

## Installing on a Chromebook

1. Open Chrome and navigate to your hosted URL
2. Click the **install icon** (⊕) in the address bar, OR
3. Click the three-dot menu → "Install ProtraxAR"
4. The app will appear in your app launcher and can be pinned to the shelf

## Installing on a Promethean Board

1. Open the built-in browser and navigate to the URL
2. Tap the install prompt that appears, OR use the browser menu
3. The app opens in fullscreen mode automatically

---

## Controls

| Action | How |
|--------|-----|
| Move protractor | Drag with finger or mouse |
| Rotate | Two-finger twist, scroll wheel, or ← → arrow keys |
| Fine rotate | Shift + ← → (15° steps) |
| Resize | Pinch gesture or Size slider |
| Snap to 15° | Enable "Snap 15°" toggle in panel |
| Reset rotation | Press R key |

---

## File Structure

```
protraxar/
├── index.html       ← Main app
├── manifest.json    ← PWA manifest
├── sw.js            ← Service worker (offline support)
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

---

## Customization

- **Colors**: Edit the swatch hex values in index.html
- **Default size**: Change `value="200"` on the size slider
- **Snap angle**: Change `Math.round(rotation / 15)` to a different divisor

---

Built for educators. Works offline once installed.
