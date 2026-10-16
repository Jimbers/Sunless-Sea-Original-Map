# The Sunless Sea: web map

A MapLibre GL web edition of the QGIS project `SunlessSea.qgz`.

- `index.html` is the whole app. MapLibre is loaded from unpkg, and labels use EB Garamond from Google Fonts.
- `data/` holds the layers, exported from `SunlessSea.gdb` and `ClansEditable.gpkg` and converted to WGS 84 GeoJSON:
  abyss, ocean, territories, clans, rivers, impassable and labels.
  `data/grad/` holds the gradient fills (Candle Tower, Demilamp and volcanoes), baked as PNG overlays.

- `downloads/SunlessSea_QGIS.zip` is the portable QGIS project (SunlessSea.qgz plus SunlessSea.gpkg), linked from the map's panel.

- `3d/` is the interactive 3D relief (three.js): terrain, light and settlements synthesised from the map data and its lore.

Hosting: push this folder to a GitHub repo, then go to Settings → Pages → Deploy from branch → `main` / root.
