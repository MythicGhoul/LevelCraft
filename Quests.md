# Quests, questlines & objectives

Quests turn ordinary survival tasks into structured adventures. LevelCraft distinguishes normal quests from promotion exams, and quest definitions can be grouped into multi-step questlines.

## Player experience

1. Open `/quests` or `/lc quests`.
2. Choose **Quests** or **Promotion Exams**.
3. Filter by available guild tier (F through S) where the interface supports it.
4. Select a questline and review the individual steps.
5. Accept an available quest, complete its objective and claim its reward.

Quest reward types include skill XP, items, economy rewards and commands. Higher ranks may introduce boss fights or other prerequisites.

## Supported objective families

| Type | Example |
| --- | --- |
| `KILL_MOB` | Defeat a specified mob type |
| `CHOP_LOG` | Harvest logs of a particular material |
| `MINE_BLOCK` / ore objective | Break eligible blocks or ores |
| `CAST_SPELL` | Cast a named spell |
| `WALK_DISTANCE` | Travel a required distance |
| `FISH_CATCH` | Catch fish |
| `FARM_HARVEST` | Harvest crops |
| `VOTES` | Complete eligible vote actions when the vote integration is active |
| Economy cost objectives | Spend a required amount through the economy integration |

The exact enum names accepted by a given JAR should be checked before editing YAML. The `quests.yml` example in [Quest configuration](https://github.com/MythicGhoul/LevelCraft/wiki/Reference-Quests-Config) uses the real `MINE_BLOCK` and `CHOP_LOG` syntax found in referenced quest data.

## Questlines

A questline is an ordered series of quests. `Quest-Line` groups steps while `Line-Order` defines order within that line. The interface can show the line first, then reveal its individual tasks. A completed prerequisite can unlock the next quest.

## Repeatable quests

Some quests can be set `Repeatable: true`, while others provide one-time progress. Repeatability affects completion tracking and claim logic, so changing it on a live server should be planned carefully.

## Troubleshooting

If a quest stays incomplete, check the objective ID, target material, active state, permission/guild tier and player progress. If a claimed reward does not run, verify the Vault economy and console command syntax as applicable.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Quests](https://github.com/MythicGhoul/LevelCraft/wiki/Quests) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
