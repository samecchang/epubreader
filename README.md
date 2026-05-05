# ePub Reader

A standalone, single-file HTML ePub reader with a modern UI and smooth page-flipping animations.

## Features

- **Single-file deployment** — No build process, no dependencies beyond CDN libraries
- **Two-column book layout** — CSS multi-column layout displays content as a book spread
- **Chapter-aware pagination** — Chapters start on new columns
- **Multiple navigation methods**:
  - Draggable progress slider
  - Page number input with "Go" button
  - Navigation buttons (◀ ▶)
  - Keyboard shortcuts (Arrow keys, PageUp/PageDown)
  - Touch swipe gestures
  - Click on left/right edges of viewport
- **Font size adjustment** — Slider and keyboard shortcuts (+/-)
- **Custom page-flipping animation** — Smooth expand effect when turning pages
- **Responsive design** — Adapts to window resize
- **Dark theme UI** — Modern dark interface with light content area

## Usage

1. Open `ePubReader.html` in a web browser
2. Click "Open" and select an `.epub` file
3. Navigate using any of the supported methods:
   - **Slider**: Drag to jump to any page
   - **Page input**: Enter page number and click "Go" or press Enter
   - **Nav buttons**: Click ◀ / ▶ to turn pages
   - **Keyboard**: Arrow keys or PageUp/PageDown
   - **Touch**: Swipe left/right on mobile devices
   - **Click**: Tap left/right 15% of viewport edges
4. Adjust font size with the Font slider or A+/A- buttons

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| → / PageDown | Next page |
| ← / PageUp | Previous page |
| + / = | Increase font size |
| - | Decrease font size |
| Ctrl + Wheel | Adjust font size |

## Technical Details

- **Libraries**:
  - [JSZip](https://cdn.jsdelivr.net/npm/jszip@3.10.1/dist/jszip.min.js) — ePub parsing
- **CSS Multi-column layout** — Uses `column-count: 2` with dynamic `column-width` calculation
- **Pagination** — Each column is treated as a "page" (left = page N, right = page N+1)
- **Animation** — Custom expand effect using cloned DOM elements with `scrollLeft` navigation

## Browser Compatibility

Works in modern browsers that support:
- CSS Multi-column layout
- ES6 JavaScript
- CSS Grid/Flexbox

## License

MIT License

## Author

Created as a standalone ePub reader for personal use.
