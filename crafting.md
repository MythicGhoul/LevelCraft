# Crafting

**Creating equipment, building supplies and food recipes.**

## How to earn Crafting XP

Craft eligible recipes and food; fulfil crafting objectives.

Every XP source has eligibility checks, and award amounts may vary by material, entity, action, environment and the installed build. Use the character sheet to confirm a real increase rather than relying only on the action-bar animation.

## Milestones and rewards

Crafting-focused mastery and broader resource economy utility. See [Skill milestones](../milestones.md) for the common level-10, level-25, level-40 and level-50 framework. The actual perk names, odds and values come from the currently installed code and YAML.

## Practical tips

- Train through normal survival activities instead of farming a single low-value action indefinitely.
- Check [Total Level](../leveling.md) as the skill improves; Total Level affects broader combat and item effectiveness.
- Look for [Quest](../../quests/overview.md) steps involving this activity, which may award extra skill XP.
- Some world events and prestige benefits modify eligible XP awards.

## Detailed Crafting mechanics

### Recognised recipes
Crafting can cover food creation and ordinary recipes as well as configured special items. The plugin needs to distinguish actual crafted results from moving finished items around an inventory.

### Shift-click behaviour
Bulk crafts can legitimately produce several items in one click. A correct XP award should scale or cap as intended and avoid crediting the same recipe repeatedly through inventory refreshes.

## Known interactions

Repetitive crafting may be subject to server balancing and item restrictions.

## Checking a scoreboard value

```text
%levelcraft_skill_crafting_level%
%levelcraft_skill_crafting_xp%
%levelcraft_skill_crafting_xp_required%
%levelcraft_skill_crafting_progress_percent%
```

These require the optional PlaceholderAPI integration. See [Placeholder reference](../../reference/placeholders.md).

---

[← Documentation contents](../../README.md) · [Project homepage](../../../README.md)
