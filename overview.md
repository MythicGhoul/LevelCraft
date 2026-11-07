# Server administration

LevelCraft includes a broad in-game admin surface for maintaining progression systems, creating NPCs, managing quests, testing structures and adjusting player state. This section is aimed at server owners and trusted moderators.

## Recommended rollout order

1. Confirm plugin dependencies and first-boot configuration.
2. Check a new player's race/path onboarding experience.
3. Establish appropriate XP gain, health, damage and mob scaling.
4. Configure F-rank quests and a clear first promotion experience.
5. Place essential NPC shops and guide signage.
6. Validate rare equipment, Power Level and socket costs.
7. Add shrines, bosses, corruption and encounter scheduling.
8. Enable maps, Discord alerts, vote systems and other integrations.
9. Back up the data and test a full server restart.

## Useful admin interfaces

- `/lc admin` opens the administration UI on supported builds.
- `/lc admin quests editor` opens the quest editor.
- `/lc admin shrine spawn` tests shrine placement near a player.
- `/lc admin reload` reloads supported configuration files.
- The NPC editor can be reached through the admin GUI and, in referenced NPC data, `/lc admin villager`.

## Do not debug on production first

Prepare a small test world with one fresh account and one experienced account. Keep a separate backup of real player inventories and quest progress before testing changes to persistent item or character data.

[Backups](backups.md) · [Performance](performance.md) · [Troubleshooting](troubleshooting.md) · [Security](security.md)
