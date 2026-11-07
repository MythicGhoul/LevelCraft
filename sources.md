# Documentation sources & version status

This documentation package was assembled using public LevelCraft information and project materials from previous development sessions. It is designed as a **substantial initial documentation collection**, not as a claim that every implementation detail has been verified against the newest compiled JAR.

## Main sources

- [Public LevelCraft GitHub repository](https://github.com/MythicGhoul/LevelCraft): repo identity and existing EPL-2.0 licence; public repo has not contained the plugin implementation itself at the time of this documentation build.
- [SpigotMC LevelCraft resource](https://www.spigotmc.org/resources/110629/): public feature overview and published plugin positioning.
- [MythicSuite website](https://mythicsuite.co.uk/): ecosystem positioning and product information.
- Internal project materials referenced during authoring: `plugin.yml` version **6.4.2**, `LevelCraftCommand(9).java`, `LevelCraft_Placeholders.java`, `config(10).yml` (November 2026), `quests(4).yml` and `VillageTrade_all_town_shops.yml`.
- Earlier feature-by-feature development notes and design decisions covering updates through November 2026.

## Verification grades

**Registered/confirmed:** A command or key present in a referenced manifest, handler or YAML extract.

**Documented design:** A feature described or developed in prior project work; its shipping status can depend on build.

**Server-specific:** A configurable NPC, objective, boss, encounter or balance value that may differ per installation.

## How to keep docs authoritative

After each LevelCraft release, export the active `plugin.yml`, current config defaults, real command help, item registry and feature states; review changed pages and remove any stale entries. This avoids mixing old ideas with currently shipped gameplay.

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
