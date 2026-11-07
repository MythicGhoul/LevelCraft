# All 11 skills

Every LevelCraft character progresses in **eleven** skills. Skills award XP from relevant survival actions and provide milestone benefits. The level screen is reached through the character interface; the `skill_*` PlaceholderAPI family is available for scoreboards and HUDs.

| Skill | Core activity |
| --- | --- |
| [Combat](https://github.com/MythicGhoul/LevelCraft/wiki/Skill-Combat) | Fighting hostile mobs and bosses |
| [Mining](https://github.com/MythicGhoul/LevelCraft/wiki/Skill-Mining) | Ores, stone and mineral gathering |
| [Woodcutting](https://github.com/MythicGhoul/LevelCraft/wiki/Skill-Woodcutting) | Trees, logs and timber |
| [Farming](https://github.com/MythicGhoul/LevelCraft/wiki/Skill-Farming) | Crops and animal husbandry |
| [Fishing](https://github.com/MythicGhoul/LevelCraft/wiki/Skill-Fishing) | Catching and fishing events |
| [Hunting](https://github.com/MythicGhoul/LevelCraft/wiki/Skill-Hunting) | Tracking and defeating creatures |
| [Smithing](https://github.com/MythicGhoul/LevelCraft/wiki/Skill-Smithing) | Processing and enhancing gear |
| [Exploration](https://github.com/MythicGhoul/LevelCraft/wiki/Skill-Exploration) | Travel and discoveries |
| [Excavation](https://github.com/MythicGhoul/LevelCraft/wiki/Skill-Excavation) | Digging blocks and terrain |
| [Crafting](https://github.com/MythicGhoul/LevelCraft/wiki/Skill-Crafting) | Making items and food |
| [Sorcery](https://github.com/MythicGhoul/LevelCraft/wiki/Skill-Sorcery) | Mana, spells and wands |

## Reading your progress

Open `/stats` for the character sheet or use the corresponding GUI from `/lc stats`. The exact per-skill earned XP and required XP can also be accessed through placeholders such as `%levelcraft_skill_mining_level%` and `%levelcraft_skill_mining_xp%`.

## Why some actions award no XP

Activity filters may protect against farms, exploit loops or re-placed resource blocks. The admin config and relevant skill listener determine which actions count. For troubleshooting, test the same action outside spawn, with an ordinary vanilla block and an unmodified tool.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Progression](https://github.com/MythicGhoul/LevelCraft/wiki/Character-Progression) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
