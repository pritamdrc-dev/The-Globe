# Atlas Globe

A full-viewport 3D globe built with three.js: glowing markers, drag-to-spin with inertia,
click-to-focus with smooth camera transitions, atmosphere glow, and auto-rotate that pauses
while you interact.

## Run

```bash
git init && git add . && git commit -m "Atlas Globe"
npm start            # serves on http://localhost:3000
# or: python3 -m http.server 3000
```

Any static server works. Opening `index.html` directly may block the Earth texture in some browsers.
Three.js, the Earth texture and fonts load from CDNs (jsdelivr, cdnjs, Google Fonts), so an internet connection is needed.

## Customize

- Locations: edit the `LOCATIONS` array at the top of the script in `index.html` (name, country, lat, lon, desc).
- Rotation speed and resume delay: `AUTO` and `RESUME_AFTER`.
- Marker colour: `COL` / `COL_ON`.

## Controls

Drag to spin, scroll or pinch to zoom, click a marker or list item to focus, Esc or empty space to release.
