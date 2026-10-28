# Legacy map system — final snapshot (2026-10-28)

The Surviving Adamsville map system exactly as it stood in
kingmarkarnold-code/adamsville-play @ f1ac88af43c6e27e8ab131d5d3bd5a39a2aff648
(main HEAD, 2026-10-28) immediately before the Adamsville redraw programme
replaced it: all seven zones' data under detailed/zones/, the map manifest,
and the map-serving code (zoneloader, zoneunlock, zoneunlockflow,
mapdelivery, road/terrain/water sync, gps, traffic).

Branch: legacy-map-final-2026-10-28 in adamsville-play-archive.
A byte-identical local copy + per-file sha256 manifest lives at
~/workspace/game-map/backups/2026-10-28-legacy-map-final/ (SNAPSHOT-MANIFEST.json).

Restore = take the tree of this branch; paths are repo-relative (detailed/...).
