# All 11 skills

Every LevelCraft character progresses in **eleven** skills. Skills award XP from relevant survival actions and provide milestone benefits. The level screen is reached through the character interface; the `skill_*` PlaceholderAPI family is available for scoreboards and HUDs.

| Skill | Core activity |
| --- | --- |
| [Combat](combat.md) | Fighting hostile mobs and bosses |
| [Mining](mining.md) | Ores, stone and mineral gathering |
| [Woodcutting](woodcutting.md) | Trees, logs and timber |
| [Farming](farming.md) | Crops and animal husbandry |
| [Fishing](fishing.md) | Catching and fishing events |
| [Hunting](hunting.md) | Tracking and defeating creatures |
| [Smithing](smithing.md) | Processing and enhancing gear |
| [Exploration](exploration.md) | Travel and discoveries |
| [Excavation](excavation.md) | Digging blocks and terrain |
| [Crafting](crafting.md) | Making items and food |
| [Sorcery](sorcery.md) | Mana, spells and wands |

## Reading your progress

Open `/stats` for the character sheet or use the corresponding GUI from `/lc stats`. The exact per-skill earned XP and required XP can also be accessed through placeholders such as `%levelcraft_skill_mining_level%` and `%levelcraft_skill_mining_xp%`.

## Why some actions award no XP

Activity filters may protect against farms, exploit loops or re-placed resource blocks. The admin config and relevant skill listener determine which actions count. For troubleshooting, test the same action outside spawn, with an ordinary vanilla block and an unmodified tool.

---

[← Documentation contents](../../README.md) · [Project homepage](../../../README.md)
