# Developer architecture

The documented LevelCraft project is a Java plugin targeting the Bukkit/Spigot family. A referenced entry point is:

```java
package me.Ghoul.LevelCraft;

public class Main extends JavaPlugin {
    // plugin lifecycle and manager wiring
}
```

This fragment is **illustrative**, not a verbatim excerpt from the Java source. Its class/package identity is supported by the referenced `plugin.yml`.

## Package layout philosophy

The project convention keeps only the Main entrypoint in `me.Ghoul.LevelCraft`, with feature packages at the project root (for example commands, listeners, managers, gui, utils and models). Recent source snapshots also show packages such as `ExpSystem`, `Structures`, `Utils` and related feature groupings.

## Representative subsystem groups

| Domain | Responsibilities |
| --- | --- |
| Player progression | Skill XP, milestones, Total Level, races, paths and prestige |
| Combat & items | Damage scaling, rarity, Power Level, sockets and custom item data |
| Quest system | Definition loading, objective tracking, claims and reward execution |
| World simulation | Mob scaling, corruption, shrines, roaming encounters and bosses |
| Economy & NPCs | Vault transactions, shops, item serialization and managed villagers |
| Social | Parties, clans, permissions and item trades |
| Presentation | Character GUIs, nametags, PlaceholderAPI and map overlays |
| Persistence | YAML files, profile data, locations and state restoration |

## Event design

Keep event listeners small and delegate business rules to managers. Avoid performing heavy disk I/O, large block writes or expensive entity scans in frequent synchronous handlers. Validate all custom item metadata on the server, not by display name alone.

## Dependencies and startup

Vault is a hard dependency in the referenced manifest; optional integrations should be registered only after confirming their plugins and APIs are available. Placeholders and map hooks may need explicit registration and state replays after data loading.

## Builds

The project is managed as an **Eclipse-style non-Maven source project** in the documented workflow. This documentation itself is unrelated to the Java build tool and can be published without distributing plugin code.

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
