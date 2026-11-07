# Roaming world encounters

Roaming encounters introduce occasional enemy groups outside dedicated arenas. The November 2026 configuration provides a `World-Encounters` section with global toggles, per-player checks, cooldowns, spawn-distance restrictions and individual themed encounters.

## Encounter families in the referenced config

- **Undead Patrol:** zombies, skeletons and husks.
- **Slime Swarm:** groups of slimes.
- **Spider Nest:** spiders and cave spiders.
- **Skeleton Warband:** skeleton and stray variants.
- **Pillager Scouts:** pillagers and vindicators.
- **Nether Incursion:** zombified piglins, magma cubes and blazes.
- **Ender Pack:** endermen and endermites.

These are configuration-defined encounter families; server owners can disable or re-balance them independently.

## Example control settings

```yaml
World-Encounters:
  Enabled: true
  Check-Interval-Seconds: 25
  Spawn-Chance-Per-Player: 0.08
  Per-Player-Cooldown-Seconds: 600
  Min-Spawn-Distance: 35
  Max-Spawn-Distance: 70
  Spawn-Protection-Radius: 200
  Avoid-Clan-Claims: true
  Max-Active-Global: 20
  Max-Active-Near-Player: 1
```

These values are taken from a referenced project configuration and should be compared with the live file.

## Balancing advice

For low-end clients or small servers, keep per-player density and simultaneous encounter limits conservative. Distance, spawn attempts and nearby-mob caps are as important as the probability of an encounter.

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
