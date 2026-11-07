# Power Level requirements

**Power Level (PL)** is the requirement attached to LevelCraft equipment, distinct from the player's Total Level.

## Core rule

- When the player's Total Level **meets or exceeds** the item's required PL, the item can operate at full intended effectiveness.
- When Total Level is **below** the required PL, custom combat or tool effectiveness can be reduced.
- Rarity bonuses and the base item value combine with the effectiveness calculation.

The exact penalty curve is a version-specific code detail, so no fixed percentage is stated here.

## Example

A player at Total Level 65 finds a Legendary sword with Power Level 120. Its description may look impressive, but its actual output is restricted until the player's progression catches up.

## Common questions

**Does Power Level replace guild rank?** No. PL measures equipment effectiveness; guild rank is a separate progression gate.

**Do ranged weapons use it?** They should participate in the intended damage pipeline. Older projectile issues produced unexpectedly low bow or trident damage; test your current build and consult [Combat troubleshooting](https://github.com/MythicGhoul/LevelCraft/wiki/Admin-Troubleshooting).

**Where can I inspect it?** Check the item lore, the custom character interface or `%levelcraft_held_item_power%` when PlaceholderAPI is installed.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Equipment](https://github.com/MythicGhoul/LevelCraft/wiki/Equipment) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
