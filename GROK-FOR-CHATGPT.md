# Package for ChatGPT — LITTLE MIND / LIVING CITY

From Grok on Danny’s PC. **Inspect before modifying.** Layered Town v6 is the baseline. This is not a greenfield design.

You already stated the right stance. This file is the inventory + architectural fit, not a rewrite brief.

Full zip with 61 jpgs lives on Danny’s Desktop as `LITTLE-MIND-GROK-FOR-CHATGPT.zip`. This markdown is the same briefing without binaries.

## Canonical
- Game: `game/little-mind-layered-town-v6.html` (99697 bytes, 2026-08-26 21:12)
- Camera: `_ref/camera-grammar.txt`
- Style lock only: 09_04_42 pixel city sheet. No cozy isometric Frog Mart.
- Art: 61 jpgs in `pieces/`
- Repo: this repo, branch `dd-main`
- Not this project: Bárbara academy ZIP

## Grok did / did not
Did: park cozy look; lock cyberpunk sheet; generate 61 graphics; public repo; did not change sim.
Did not: wire pieces into canvas; embed jpgs in one HTML; guarantee alpha/tile/shared perspective; upload all binaries here.
**Art exists; live game does not yet display it.**

## Do not break
`canonicalSimulationUnchanged`, `visualResolutionFollowsBean`, TEMPLATE+SEED+VERSION+MUTATIONS, finite stocks/flows, cadastral under beautiful world, entity ids (`home`, `shop`, `cafe`…), save key `little-mind-layered-town-v6`.
APP.template is `blank` while runtime is living-city — pre-existing quirk; do not wipe the runtime to “fix” diagnostics.

## Trap
Many jpgs are hero illustrations: full scenes, no alpha, mixed aspect. They must not dictate architecture. Registry → templates → layer renderer → resolution manager → affordances. Do not `drawImage` a whole apartment jpg over `ROOM_TEMPLATES`.

## First pass
1. Confirm sim: town mode, fridge, grocery, save/load.
2. Mark each piece registry / reference-only / reject.
3. Then propose a visual asset registry. Zero TOWN_SYSTEMS changes for prettier graphics.
