# Installation & requirements

LevelCraft is a server-side Bukkit/Spigot-style plugin. Install the build that matches your Minecraft server API; the referenced development manifest identifies `me.Ghoul.LevelCraft.Main` and declares `api-version: 26.3` for that particular build.

## Dependencies

| Component | Status | Purpose |
| --- | --- | --- |
| Vault | **Required** in the referenced `plugin.yml` | Economy services for NPC purchases, quest costs and other currency features. |
| Economy provider | Required for economy features | Vault is an API bridge; provide a compatible economy implementation. |
| PlaceholderAPI | Optional | Makes LevelCraft values available in scoreboards, tab lists and other plugins. |
| Dynmap | Optional | Web-map overlays where configured. |
| BlueMap | Optional | Map markers for supported world systems. |
| WorldEdit / FastAsyncWorldEdit | Optional, feature-dependent | Supports schematic-based shrine/world-structure workflows. |
| MythicEnchant | Optional | Integration points for custom enchantments/items where supported. |

> **Compatibility**
>
> Minecraft/Spigot versions can change quickly. A release's exact supported server versions must be verified against that release; a `26.3` development manifest does **not** guarantee compatibility with older builds or non-Spigot forks.


## Install steps

1. Stop the server and back up its world and plugin data.
2. Install the correct LevelCraft JAR in `plugins/`.
3. Install Vault and a compatible economy implementation. Add optional integrations only if needed.
4. Start the server once so LevelCraft can generate its files.
5. Open the generated `plugins/LevelCraft/` directory. Read the actual files and defaults before changing them.
6. Grant player permissions through your permissions plugin when necessary. The development `plugin.yml` includes player defaults, but a server-wide policy may override them.
7. Configure race/path selection areas, NPCs, quests, world events and spawn protection for your intended experience.
8. Restart after changing startup-only integrations or dependencies; use `/lc admin reload` only for settings the running build actually reloads.

## First-launch checklist

- `/lc stats` opens the character sheet.
- `/lc quests` opens quests.
- A new player can complete the intended race and path flow.
- Money transactions work through Vault.
- A player earns skill XP from an ordinary eligible action.
- Optional map and PlaceholderAPI integrations load without errors.

## Updating safely

Copy both the old JAR and the entire `plugins/LevelCraft/` data folder somewhere safe. Replace the JAR, review newly generated or migrated YAML keys and test in staging. Do not blindly replace customised data files with defaults. See [Updates & backups](https://github.com/MythicGhoul/LevelCraft/wiki/Admin-Backups).

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Getting Started](https://github.com/MythicGhoul/LevelCraft/wiki/Getting-Started) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
