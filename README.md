# 2.5D Isometric Game Engine — World Editor

Browser-based isometric tile/object/collision editor (Three.js). Single file: `index.html`.

**Live:** https://hannes423-debug.github.io/2.5D-Isometric-Game-Engine/

## Run locally
Open `index.html` in a modern desktop browser (needs internet once for Three.js from cdnjs), or serve the folder with `npx serve`.

## Controls
- Wheel: change active height level (Ctrl+wheel: zoom) · Middle/right-drag: pan
- V select · B paint · G rect fill · X rect erase · E erase · O place object · C collision paint · I eyedropper · H pan
- R rotate · Delete remove · [ ] or PageUp/PageDown height · Ctrl+Z / Ctrl+Y undo/redo · Ctrl+S save JSON

## Files
- Save/Open: versioned JSON project. Export adds a `nav` section (walkable floors, blocked cells) for a runtime.
- Autosave goes to browser localStorage (per site, so it does not carry over between hosts).
- Coordinates: x east, y south, z up; a tile at layer z has its walking surface at elevation z+1.
