# Cleanup 2026-10-28 — local-mirror residue archived from detailed/

Moved here by the full system audit + repo cleanup (Joshua's directives 4-5,
2026-10-28). These nine files existed ONLY in the local mirror
(~/workspace/game-map/play/detailed/) — they were never in the live
adamsville-play repo (verified blob-by-blob against HEAD e27e134b) and are
referenced by nothing in the game, the editors, or the watcher
(tools/check_inventory.py full-tree run: the only 9 orphans, 0 dangling).
A copy always exists: this folder. terrain_lifts.js and junction_pins.js
also remain in the local tree as pipeline working files.

| file | bytes | sha256 | note |
|---|---|---|---|
| 535-building-editor-entry.json | 1291 | a72051fe2dff98ea03ef6ff1805e57ba72edf0b8f21f762d94ae7f24ce618115 | Building Editor 2.0.7 entry artifact; regenerates on editor use |
| building_spawner.js | 31967 | 592897764044c3e2a10495d7d1e3782b3ba8eb4f66e2f7cadbabacf4700d1e47 | Superseded spawner stub; live spawner is inline in index.html |
| icon-watcher.png | 80478 | 2be954e83942bc1cb730544d5aa79f39f6d65ca1cd2c2bf47b375b85e2907ad9 | Watcher icon asset; no reference anywhere in play or watcher repos |
| junction_pins.js | 1129923 | b1df27b20a55e9c5a5d17ad40951ee6942edfddbf05e49d20818c6e03fb3a5e2 | Hand-authored junction pins; superseded by package pins.json (kept locally too) |
| road_sync.js | 13255 | ce36818f1ca773c98218e0bd945cdae570874fbc60332493ea26eca71d82e5f4 | Retired RELEASE-SYNC pull tool copy (retirement 2026-10-09) |
| split-zones.py | 22592 | 98ed1c85c37ec4b55fae0f4235fbd8a06b60f3b2c58177fa5d6b95e96480ca5c | Zone-split tool; repo keeps proto-maps/split-zones.py |
| terrain_lifts.js | 561214 | f19191e0c26d5710c960c59c475a077d97279c7b4d339f1590fb33b5f78a0cbb | Pre-conversion fossil per AGENTS.md; per-zone lifts.js are the live form (kept locally too) |
| terrain_sync.js | 8403 | 059bdd0d517e2b39fecc7c973a429298e4f4140aee967f8286f3cc4147f112cd | Retired RELEASE-SYNC pull tool copy (retirement 2026-10-09) |
| watcher-final.png | 80478 | 2be954e83942bc1cb730544d5aa79f39f6d65ca1cd2c2bf47b375b85e2907ad9 | Watcher screenshot artifact, 2026-10-12 |
