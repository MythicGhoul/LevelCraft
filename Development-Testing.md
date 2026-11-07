# Testing and release checklist

A change is not ready for production until it survives both real gameplay and plugin lifecycle events.

## Functional test matrix

| Category | Minimum test |
| --- | --- |
| First join | New player chooses race/path once and receives only the configured kit. |
| XP | Same activity grants proper normal, event and party XP. |
| Gear | Rarity, Power Level, enchants and gems survive inventory transfers. |
| Quests | Accept, progress, fail/leave, claim, repeat and save/reload. |
| Magic | Learn, loadout, cast, cooldown and mana recovery. |
| World | Shrine spawn/collapse, corruption grow/cleanse, boss death and restart. |
| Economy | Buy, sell, insufficient funds, full inventory and bulk quantity. |
| Clans | Permissions, claim flags and anti-grief protection. |
| Trade | Cancel, reconnect, both-confirm and custom item integrity. |
| UI | Menus, placeholders and nametags for two concurrent players. |
| Upgrade | Migration backup, fresh default config and rollback. |

## Stress testing

Add multiple concurrent players, large inventories, many active entities and repeated world load/unload cycles. Profile real work with a server profiler rather than relying only on success messages.

## Release documentation

For each released build, record:

- Version number and Minecraft/API compatibility.
- Added/removed command syntax.
- New or migrated config keys.
- Player data schema changes.
- Known limitations and changed balance.
- Whether the documented features are stable, beta or experimental.

Use [Documentation sources](https://github.com/MythicGhoul/LevelCraft/wiki/About-Sources) as the provenance point when updating these guides.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Development](https://github.com/MythicGhoul/LevelCraft/wiki/Development) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
