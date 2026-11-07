# Managed NPC shops

LevelCraft can manage world NPCs for buying, selling, services, guild exchanges and dialogue. The referenced setup uses a separate `VillageTrade.yml` file for its NPC definitions and trading rules.

## Shop roles

| NPC / shop type | Examples |
| --- | --- |
| Guild | Guild Master Aldric, Clerk Mira |
| Weapon smith | Weapons and rarity-based inventory |
| Armour smith | Garrick and armour selection |
| Tool smith | Bromm and work tools |
| Magic shop | Wands, tomes, special items and souls |
| Farmer / Fisherman | Flat categories of survival products |
| Guild loot buyer | Buys configured custom loot items |
| Dialogue-only NPC | Conversations without a shop transaction |

NPC names and available items are **server data**, not universal plugin defaults.

## Using a shop

1. Interact with the NPC.
2. Choose the main shop category or rarity tier.
3. Pick an eligible item and inspect the price.
4. Adjust the purchase amount if the configured GUI supports bulk selections (such as 1, 32 or 64).
5. Confirm that you have enough balance and inventory space.

## Admin controls

The referenced village configuration recommends `/lc admin villager` or the LevelCraft admin GUI. Because the subcommand set can change, use the in-game editor to create NPCs, select functions, edit shop pages and inspect stock.

### Important YAML sections

`VillageTrade.yml` contains `Settings`, `Settings.Generated-Shops` and `NPCs` in the referenced data. Its generated shops include rarity multipliers, material pricing, magic spell prices, socket gems, misc items and enchantment categories.

Read [VillageTrade configuration](../reference/npc-config.md) for a real example.

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
