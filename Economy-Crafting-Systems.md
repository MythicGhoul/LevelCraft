# Crafting systems & transmutation

LevelCraft combines standard crafting and custom progression systems. Different installations may enable dedicated crafting rooms, special furnaces, unique recipes and transmutation equipment.

## Custom recipes

Recipes may reference custom LevelCraft items, forge-related materials, soul objects or utility items. Recipe displays in a map room are useful for players, but the definitive inputs should come from the registered recipe in the installed build.

## Special furnaces

Referenced LevelCraft administration supports a furnace-item command family:

```text
/lc admin furnace list
/lc admin furnace <player> <tier/all> [amount]
```

Custom furnaces may implement enhanced output or processing effects. Do not assume furnace tiers or recipes without checking their live tooltip and config.

## Transmutation chest

The transmutation system has a balance value exposed as `%levelcraft_transmutation_balance%` in the documented PlaceholderAPI expansion. Its exact recipe, currency rules and item conversion catalogue are build-specific; consult the in-game recipe viewer for your installed version.

## Recommended admin tests

- Ensure custom recipes return the expected **PDC-backed** LevelCraft result.
- Confirm furnace data survives restarts.
- Prevent shift-click crafting from bypassing quantity and item metadata checks.
- Verify custom-item conversion cannot duplicate currency or equipment.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Economy](https://github.com/MythicGhoul/LevelCraft/wiki/Economy) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
