# Runtime (canonical v6 on this PC)

Play locally: http://127.0.0.1:8875/cyber/

File: `game/little-mind-layered-town-v6.html` (comma-fixed `loadGfx` / `visualFor` / `drawSprite`).

## VISUAL_ASSETS

```
building:
  cafe        sprites/code-cafe.png
  grill       sprites/code-grill.png
  office      sprites/code-office.png
  shop        sprites/code-shop.png
  clinic      sprites/code-clinic.png
  school      sprites/code-school.png   # matte still dirty
  warehouse   sprites/code-warehouse.png
  apartment   sprites/cutout-hotel.png  # high-rise stand-in
  vacant      sprites/cutout-vacant-forsale.png
layer:
  mountains   sprites/parallax-mountains.png
  signs       sprites/pack-signs.png    # sheet, not split
  vehicles    sprites/pack-vehicles.png # sheet, not split
```

`drawBuilding` uses the sprite if loaded, else the old procedural path. `TOWN_SYSTEMS` / fridge / jobs / `compileRoom` unchanged.

Town `view-town-*.jpg` are **not** the Town View. Palette/reference only.

## What is on GitHub vs disk

- This repo: HTML + docs + camera grammar + 480px **previews** under `sprites/preview/` when they fit the file API.
- Full RGBA sprites and 61 source jpgs stay on Danny’s PC (`Desktop/CYBER TOWN/sprites`, `pieces/`). Too large for the file API.

## Next (Pass A objects)

Map extracted furniture/fridge/elevator sheets onto `OBJECT_TEMPLATES` **after** the game is confirmed to render (hard refresh). Do not overlay a whole room JPG on the interaction graph.
