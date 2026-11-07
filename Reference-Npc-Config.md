# NPC shop YAML reference

The managed NPC system uses a separate `VillageTrade.yml` containing settings, generated shop pricing and per-NPC records.

## Real configuration structure

The referenced project shop data begins with settings such as:

```yaml
Settings:
  Default-Shop-Title: '&8%npc%'
  Default-Guild-Buyer-Title: '&8Guild Exchange - %npc%'
  Default-Farewell: '&aHappy adventuring, &f%player%&a!'
  Look-At-Players:
    Enabled: true
    Range: 8.0
    Update-Ticks: 4
  Generated-Shops:
    Equipment:
      Rarity-Multipliers:
        COMMON: 1.0
        UNCOMMON: 1.75
        RARE: 3.5
        EPIC: 7.5
        LEGENDARY: 15.0
        MASTERCRAFT: 30.0
      Material-Base:
        WOODEN: 150.0
        STONE: 300.0
        IRON: 900.0
        DIAMOND: 3500.0
        NETHERITE: 9000.0
```

This is a **short extract**, not a complete drop-in replacement. Other price keys and categories are omitted deliberately.

## Settings families

- **Look-At-Players:** NPC head-tracking distance and update cadence.
- **Generated-Shops.Equipment:** material pricing, rarity and item type multipliers.
- **Generated-Shops.Magic:** tome/spell and magical shop pricing.
- **Generated-Shops.Socket-Gems:** tier-based gem costs.
- **Generated-Shops.Misc:** utility items, bombs, forge cores and special furnaces.
- **Generated-Shops.Enchantments:** enchantment filtering and price scaling.
- **NPCs:** per-villager location, appearance, function, custom pages and buy-back lists.

## Managing custom items

Shop items may use a complete Bukkit `ItemStack` serialization rather than a simple material name. This preserves custom plugin metadata and enchantments. Prefer the in-game editor for complex items.

## Common problems

If a shop is visible but not selling, check the NPC function, category, price, Vault provider, item serialization, stack amount and inventory capacity. If a guild loot buyer is absent, inspect both NPC type settings and the `Guild Buyer` configuration options.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Reference](https://github.com/MythicGhoul/LevelCraft/wiki/Reference) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
