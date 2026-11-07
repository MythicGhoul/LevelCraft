# Smithing

**Improving equipment and working with furnaces or forged materials.**

## How to earn Smithing XP

Use permitted smithing and processing actions; engage with upgrade systems.

Every XP source has eligibility checks, and award amounts may vary by material, entity, action, environment and the installed build. Use the character sheet to confirm a real increase rather than relying only on the action-bar animation.

## Milestones and rewards

Industrial specialisation and equipment progression. See [Skill milestones](../milestones.md) for the common level-10, level-25, level-40 and level-50 framework. The actual perk names, odds and values come from the currently installed code and YAML.

## Practical tips

- Train through normal survival activities instead of farming a single low-value action indefinitely.
- Check [Total Level](../leveling.md) as the skill improves; Total Level affects broader combat and item effectiveness.
- Look for [Quest](../../quests/overview.md) steps involving this activity, which may award extra skill XP.
- Some world events and prestige benefits modify eligible XP awards.

## Detailed Smithing mechanics

### Smithing vs. forging
Ordinary Smithing XP sources and LevelCraft's rarity-upgrade forge are different workflows. The forge can add rarity and Power Level progression while smithing focuses on the player's craftsmanship.

### Item safety
When modifying weapons and armour, preserve existing enchants and persistent metadata. An upgrade should never silently downgrade a recognised custom item to an ordinary vanilla copy.

## Known interactions

The custom forge and ordinary vanilla smithing are related but not interchangeable.

## Checking a scoreboard value

```text
%levelcraft_skill_smithing_level%
%levelcraft_skill_smithing_xp%
%levelcraft_skill_smithing_xp_required%
%levelcraft_skill_smithing_progress_percent%
```

These require the optional PlaceholderAPI integration. See [Placeholder reference](../../reference/placeholders.md).

---

[← Documentation contents](../../README.md) · [Project homepage](../../../README.md)
