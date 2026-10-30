# India 3D Map

India ka **3D map** — har rajya ek extruded 3D slab ki tarah, drag se ghumaya ja sakta hai, pinch/scroll se zoom.

Live: **https://rewpal5-dotcom.github.io/India-3D-Map/**

## Abhi kya hai (v0.1 — starter)

- 36 rajya / kendra shasit pradesh, asli border data se (simplified, 131 KB)
- 3D extrusion — har rajya ki deewar aur top face, depth ke hisaab se sahi order
- **Drag** se rotate, **pinch / scroll** se zoom, auto-rotate toggle, reset
- Hover par rajya ka naam, tap/click par neeche panel (naam + bbox)
- Koi library nahi — poora renderer khud likha hua (canvas 2D + apna 3D projection), koi internet dependency nahi
- Single file (`index.html`) — jahan chahein host karein, offline bhi chalta hai

## Aage kya add hoga (aapke batane par)

- Rajya par click → **ghatnaayein / jankari** (events, yojanaayein, data)
- 3D models / markers (jaise sheher, nadi, pahaad)
- Timeline slider — "us saal kya hua" wala view
- Search + rajya list
- APK (offline app) jab final ho jaye

## Tech

Vanilla JS · Canvas 2D renderer · apna perspective projection + painter's algorithm · GeoJSON (simplified)
Data: geohacker/india states GeoJSON se simplify kiya gaya.

## License

MIT
