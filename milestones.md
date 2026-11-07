# Skill milestones & discoveries

Skills are more than numbers. Milestone rewards provide new reasons to specialise and make progression noticeable in play.

## Typical skill milestone points

| Skill level | Role |
| --- | --- |
| 10 | Early specialisation bonus |
| 25 | More significant ability or efficiency improvement |
| 40 | Advanced perk or upgraded effect |
| 50 | Mastery-tier benefit |

Rewards vary by skill and installed version. For example, Woodcutting can interact with Tree Feller, Mining can unlock new processing rewards, and Sorcery increases magic capacity and effectiveness.

## Discoveries

LevelCraft tracks first-time achievements such as new biome discoveries, creature kills and fishing catches. This provides progression beyond repetitive XP grinding and contributes to the character sheet.

Discovery progress is generally stored persistently, including records in `discoveries.yml` in referenced builds. A player should only receive the relevant *first discovery* benefit once under that character's tracked data.

## EXP crystals

An ore drop system can produce **skill EXP crystals** as special amethyst-shard items. A crystal contains a skill identity in persistent item data and awards a configured XP amount when used. Servers can apply texture-pack variants for different skills.

Avoid copying a crystal's display name onto a normal item and assuming it will work: the item uses internal metadata. See [Custom items](../economy/custom-items.md).
