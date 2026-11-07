# Custom items, bombs & EXP crystals

LevelCraft contains items that behave differently from ordinary Minecraft materials. The underlying vanilla item may be common, but internal persistent data identifies the actual LevelCraft object and its tier.

## Item families

| Family | Examples | Role |
| --- | --- | --- |
| Consumable/mobility | Recall Stone, Void Pearl, Windstep Feather | Travel or tactical utility |
| Charms and totems | Verdant Charm I–III, Guardian Totem, Blood Pact Charm | Special effects |
| Mining/coin utility | Miner's Lucky Charm I–III, Coin Magnet I–III | Resource or pickup benefits |
| Defensive/offensive | Scuba Helmet, Volatile Grenade, Berserker Rune, Frost Core | Survivability and combat |
| Magical | Soul Lantern, Phoenix Feather, Abyssal Compass | Unique supernatural effects |
| Bombs | Six configured bomb tiers | Throwable explosive-style combat effects |
| Weapon families | Custom scythes | Alternate weapon presentation |
| XP items | Skill EXP crystals | Consumable skill rewards |

This catalogue records names and families from project development; not every item must be available in every release or server shop.

## EXP crystals

EXP crystals are typically rendered as **amethyst shards** and contain a skill identity and XP reward range. Use them by right-clicking the relevant air/block target as supported by the build. Admins configure crystal chance and minimum/maximum awarded XP in an EXP-crystal-specific YAML file.

## Bombs

The bomb family uses **fire charges** as a base item in the referenced design, with visible smoke particles and tiered effects. Test block-damage restrictions and entity interactions before enabling bombs in a protected world.

## Custom item correctness

Never recreate a custom item by copying its visible lore alone. Use the official item-creation GUI/command or the correct `ItemStack` metadata so identifiers, permissions and effects work.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Economy](https://github.com/MythicGhoul/LevelCraft/wiki/Economy) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
