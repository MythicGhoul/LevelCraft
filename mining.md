# Mining

**Breaking stone and ores, obtaining mineral resources and processing rewards.**

## How to earn Mining XP

Mine eligible ore types; explore caves; collect ore-linked EXP crystals; interact with unlockable mining mechanics.

Every XP source has eligibility checks, and award amounts may vary by material, entity, action, environment and the installed build. Use the character sheet to confirm a real increase rather than relying only on the action-bar animation.

## Milestones and rewards

Ore mastery, processing bonuses and mining milestone perks. See [Skill milestones](../milestones.md) for the common level-10, level-25, level-40 and level-50 framework. The actual perk names, odds and values come from the currently installed code and YAML.

## Practical tips

- Train through normal survival activities instead of farming a single low-value action indefinitely.
- Check [Total Level](../leveling.md) as the skill improves; Total Level affects broader combat and item effectiveness.
- Look for [Quest](../../quests/overview.md) steps involving this activity, which may award extra skill XP.
- Some world events and prestige benefits modify eligible XP awards.

## Detailed Mining mechanics

### Ore categories and processing
Ore value can influence XP and special drops. Recent LevelCraft work also tied smelting-related XP into Mining progression starting around Mining level 10. The correct source and award amount should be verified in the installed listener.

### EXP crystal drops
Some ore breaks produce consumable skill crystals. Their chance and XP range are configured independently from the ordinary Mining award. Breaking an ore and consuming its crystal are therefore two separate reward events.

## Known interactions

Some XP sources treat placed blocks differently; special ore drops are controlled by the EXP crystal configuration.

## Checking a scoreboard value

```text
%levelcraft_skill_mining_level%
%levelcraft_skill_mining_xp%
%levelcraft_skill_mining_xp_required%
%levelcraft_skill_mining_progress_percent%
```

These require the optional PlaceholderAPI integration. See [Placeholder reference](../../reference/placeholders.md).

---

[← Documentation contents](../../README.md) · [Project homepage](../../../README.md)
