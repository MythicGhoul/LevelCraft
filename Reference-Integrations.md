# Integrations

LevelCraft deliberately combines several server systems. Optional integrations are detected at runtime in the referenced build; mandatory dependencies must be available during startup.

| Integration | Role | Requirement |
| --- | --- | --- |
| Vault | Currency API | Required by referenced manifest |
| Economy plugin | Stores player balances | Needed for money features |
| PlaceholderAPI | Dynamic stats in other UIs | Optional |
| Dynmap | Web markers and territory overlays | Optional |
| BlueMap | 3D map overlays and location markers | Optional |
| WorldEdit / FAWE | Schematic placement for structures | Optional / module-specific |
| MythicEnchant | Custom enchantment/item interoperability | Optional |
| MythicVote | Vote quests and rewards | Integration-specific |
| Discord webhook | Event/alert announcements | Configurable feature |

## PlaceholderAPI

LevelCraft's expansion is designed to register as part of the plugin when PlaceholderAPI is present. Use [the placeholder catalogue](https://github.com/MythicGhoul/LevelCraft/wiki/Reference-Placeholders) to test identity, stats, mana and world values.

## Web maps

Some map hooks register existing objects on startup and then update them when state changes. Read [Dynmap & BlueMap](https://github.com/MythicGhoul/LevelCraft/wiki/World-Maps) for layer troubleshooting.

## Custom items from other plugins

Where trade windows, custom NPC shops or item rewards accept `ItemStack`s, the entire metadata must survive transfer. Test with third-party enchants and plugin-created items, not only vanilla diamonds.

## Compatibility policy

Do not promise support for a dependency version simply because its plugin name appears in `softdepend`. Test the exact version and method signatures used by the runtime adapter.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Reference](https://github.com/MythicGhoul/LevelCraft/wiki/Reference) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
