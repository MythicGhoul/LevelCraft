# Backups, updates & migrations

The LevelCraft data directory contains more than preferences. It can also contain player progression, quest completion, clan territory, structure state, NPCs, custom-shop items and discovery history.

## Backup before changing the plugin

At minimum, back up:

- The active LevelCraft JAR and its version number.
- The complete `plugins/LevelCraft/` directory.
- Relevant plugin config/data dependencies, particularly economy and permission providers.
- The affected worlds and structure-related regions.
- Any separately hosted Dynmap/BlueMap or Discord webhook configuration needed for recovery.

## Update procedure

1. Stop the server.
2. Create a dated full backup.
3. Install the matching LevelCraft build.
4. Start the server while watching its error log.
5. Compare newly added or renamed config settings to your previous YAML.
6. Validate player data, guild rank, items, shops, questlines and corruption state.
7. Test a second restart.

## Automatic config updating

Referenced LevelCraft servers have used a `config backups` directory and a migration/updater workflow. That is useful protection, but **a generated backup does not replace an independently stored server backup**.

## Rollback strategy

If an upgrade corrupts data, stop the server and restore both the matching JAR **and** the corresponding plugin data snapshot. Rolling back the JAR alone can leave a newer data schema that older code cannot read.

## Secrets and privacy

Before committing anything publicly, remove webhook URLs, database credentials, API tokens, player UUID data and private shop/location data. The documentation ZIP intentionally contains none of those values.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Administration](https://github.com/MythicGhoul/LevelCraft/wiki/Administration) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
