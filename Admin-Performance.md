# Performance & low-end clients

LevelCraft has world-level events, particles, custom entities, HUD updates and map integrations. Each can be efficient on its own, but combining them in busy areas can cause server tick pressure or client frame drops.

## Recommended priorities

| Feature | Cost risk | Practical mitigation |
| --- | --- | --- |
| Ambient particles | Client rendering | Limit per-player particle rate, radius and density. |
| Roaming encounters | Mob AI and physics | Cap active mobs globally and near each player. |
| Corruption spreading | Block updates and saving | Bound chunks per core and spread frequency. |
| Shrines | Schematic writes and collapse effects | Keep work in sensible batches and respect unloaded chunks. |
| Floating nametags | Entity/text updates | Track only nearby players and clean up on quit. |
| Web map hooks | Marker data updates | Update only changed markers rather than rebuilding all layers. |
| Boss mechanics | AI, AoE and particles | Limit concurrent bosses and effect ranges. |

## Good settings to inspect

The referenced `World-Encounters` configuration has `Max-Active-Global`, `Max-Active-Near-Player`, `Max-Encounter-Mobs-Near-Player`, check intervals and spawn cooldowns. Corruption has spread chance and max-chunk limits. These are strong starting points for performance tuning.

## Visual quality without FPS problems

Keep special magic effects concentrated around meaningful events: brief particles on casts, a richer ring on boss spawn, sparse ambient particles around cores and small collapses spread over time. A little atmosphere goes further than a constant full-screen particle storm.

## Testing methodology

1. Record the baseline TPS/MSPT and client FPS in an empty world.
2. Enable one LevelCraft module or effect at a time.
3. Test 1, 5 and 20 nearby players where feasible.
4. Compare world activity with map integrations on and off.
5. Profile slow event handlers and repeated entity loops rather than guessing.
6. Treat client FPS and server tick time as **separate** measurements.

See [Mob scaling](https://github.com/MythicGhoul/LevelCraft/wiki/World-Mob-Scaling), [Encounters](https://github.com/MythicGhoul/LevelCraft/wiki/World-Encounters) and [World events](https://github.com/MythicGhoul/LevelCraft/wiki/World-Events).

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Administration](https://github.com/MythicGhoul/LevelCraft/wiki/Administration) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
