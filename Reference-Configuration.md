# Configuration reference

LevelCraft exposes settings through YAML files in `plugins/LevelCraft/`. The exact file set and keys depend on build and which modules have been enabled. **Always start with the generated file from your installed JAR.**

## Main configuration sections

A November 2026 project `config.yml` contains these top-level groups (alongside additional groups and per-feature nested options):

| Section | Purpose |
| --- | --- |
| `Resource-Pack` | Toggle integrated resource-pack behaviour. |
| `Mob-Scaling` | Mob level and difficulty multipliers. |
| `World-Encounters` | Patrols, per-player rolls, restrictions and densities. |
| `Onboarding` | Race/path first-join flow. |
| `Clan-System` | Territory and clan-related settings. |
| `Mana-Settings` | Mana and magical progression. |
| `Blood-Moon` | Night event behaviour. |
| `Corruption` | Core spawning, spread, levels, guardians and rewards. |
| `Crafting-EXP` | Crafting-related XP rules. |
| `Souls` | Soul resource settings. |
| `Prestige` | Prestige rules and rewards. |
| `Woodcutting` | Tree abilities and XP-related settings. |
| `Excavation` | Digging progression. |
| `Mining` | Ore and mining progression. |
| `Coin-Economy` | Coins and economy-related behaviour. |

## Example: gentler early-game mobs

```yaml
Mob-Scaling:
  Enabled: true
  Max-Lvl: 550
  Spawn-Range:
    Min-Factor: 0.90
    Max-Factor: 1.10
  Progression:
    Enabled: true
    Challenge-Starts-At: 150
```

This is a **partial excerpt** and must be merged into your complete generated configuration, not used alone.

## Specialised files

| File | Use |
| --- | --- |
| `quests.yml` | Quest definitions, objective targets, lines and rewards. |
| `VillageTrade.yml` | Managed NPCs, shop prices, item lists and dialogue. |
| `BossData.yml` | Boss definitions and data where present. |
| `lang.yml` | Player-facing text and localisation. |
| `discoveries.yml` | Player discovery records in referenced builds. |
| EXP-crystal configuration | Drop odds and experience ranges; exact filename varies by build. |
| Player/quest data files | Persist progression and completed content; treat as sensitive server data. |

## Editing rules

1. Back up every file you intend to edit.
2. Preserve YAML indentation (spaces, never tab indentation).
3. Check numeric units in code comments: seconds, ticks, percentages and multipliers are **not** interchangeable.
4. Use valid Bukkit `Material` and `EntityType` names for the server version.
5. Test one setting at a time on staging.
6. Use the module-specific reload or restart when appropriate.
7. Review the auto-updater's config backups after version upgrades.

See [Quest configuration](https://github.com/MythicGhoul/LevelCraft/wiki/Reference-Quests-Config), [Shop configuration](https://github.com/MythicGhoul/LevelCraft/wiki/Reference-Npc-Config) and [Performance](https://github.com/MythicGhoul/LevelCraft/wiki/Admin-Performance).

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Reference](https://github.com/MythicGhoul/LevelCraft/wiki/Reference) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
