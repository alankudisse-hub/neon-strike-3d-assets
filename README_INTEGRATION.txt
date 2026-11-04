# NEON STRIKE 3D — CYBER FACTORY ARENA

A procedural GLB environment asset for the existing Neon Strike 3D project.

## File
- `neon_strike_cyber_factory_arena.glb`

## Intended use
Visual environment only. The deck is modeled around the existing showroom footprint (5.2 × 8.8 units). Decorative architecture surrounds the deck.

## Important integration rule
Load this model with Three.js `GLTFLoader` as a visual-only scene group. Do NOT use its meshes as gameplay colliders. Preserve the game's existing table dimensions, collision boundaries, goal positions, puck physics, paddle physics, arena IDs, shop prices, inventory, purchases and save data.

## Suggested integration
- Place the GLB in `public/assets/arenas/` or the project's existing public asset directory.
- Load it once with `GLTFLoader`.
- Clone/reuse the loaded scene for showroom and gameplay where appropriate.
- Keep gameplay collision and goal logic in the existing code.
- Adjust only visual scale/position after checking the current gameplay coordinate system.
- If decorative parts obscure the playfield, hide only those named decorative meshes; do not alter gameplay logic.

## Contents
Industrial graphite deck, layered armor rails, cyan/magenta energy strips, two visual goal frames, corner pylons, side support columns, overhead gantries, wall turbines/gears, coolant pipes, hazard markings, beacons and a central furnace reactor.
