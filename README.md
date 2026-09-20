# Flatspace — HDB floor planner

A browser-only floor planner for GitHub Pages. No build, server, account or API keys required. Floor plans stay on the user's device.

## Use

1. Upload a PNG, JPG or WebP floor-plan image (up to 25 MB).
2. Click both ends of a known wall and enter its length in metres.
3. Choose furniture or service symbols, then click to place them. Drag to move; use the Details panel to resize or rotate.
4. Draw electrical, water, aircon or lighting routes with clicks. Double-click or press Enter to finish.
5. Toggle layers, add measurements, and export a high-resolution PNG or use Print / PDF.
6. Save the editable project as JSON and reopen it later. Work is not automatically saved.

Includes furniture, electrical points, water fixtures and piping, aircon units and routes, and lighting. The initial plan is an illustrative demo, not an official HDB layout. Dimensions are planning references; uploaded drawings may contain distortion. Print uses fit-to-page and includes a scale bar, not a fixed print scale.

## GitHub Pages

In repository Settings → Pages, select **Deploy from a branch**, **main**, **/(root)**, then Save.

Expected address after Pages is enabled: https://mrscottiefy.github.io/floor_planner/

All asset paths are relative, so the app works under a GitHub Pages repository path. Open `index.html` directly for local use.

## Controls

- V: select; R: rotate selected item by 15 degrees.
- Delete / Backspace: remove selection.
- Ctrl/Cmd+Z: undo; Ctrl/Cmd+Shift+Z: redo.
- Escape: cancel placement or route; Enter: finish route.
- Mouse wheel: zoom; middle-drag or Alt-drag: pan; Fit: show the full plan.

## Files

- `index.html`: accessible editor controls and dialogs.
- `style.css`: responsive workspace and print layout.
- `app.js`: SVG editor, calibration, project validation, history, exports.
- `favicon.svg`: app icon.

No third-party runtime dependencies or external network calls.
