# Hunting

**Tracking and defeating creatures in the overworld.**

## How to earn Hunting XP

Hunt eligible wildlife or creatures; complete kill-related objectives.

Every XP source has eligibility checks, and award amounts may vary by material, entity, action, environment and the installed build. Use the character sheet to confirm a real increase rather than relying only on the action-bar animation.

## Milestones and rewards

Hunting mastery and combat-adjacent benefits. See [Skill milestones](../milestones.md) for the common level-10, level-25, level-40 and level-50 framework. The actual perk names, odds and values come from the currently installed code and YAML.

## Practical tips

- Train through normal survival activities instead of farming a single low-value action indefinitely.
- Check [Total Level](../leveling.md) as the skill improves; Total Level affects broader combat and item effectiveness.
- Look for [Quest](../../quests/overview.md) steps involving this activity, which may award extra skill XP.
- Some world events and prestige benefits modify eligible XP awards.

## Detailed Hunting mechanics

### What counts as hunting
Hunting rewards depend on which creatures and kill events are classified as eligible. Servers can balance the skill separately from hostile-mob Combat progression to avoid making one XP source dominate.

### Encounter interaction
Roaming encounter creatures and rare world spawns can be interesting hunting targets, but their entity metadata should be checked before granting quest or skill rewards.

## Known interactions

Hunting and Combat are distinct skills; the same kill may be routed differently depending on entity type.

## Checking a scoreboard value

```text
%levelcraft_skill_hunting_level%
%levelcraft_skill_hunting_xp%
%levelcraft_skill_hunting_xp_required%
%levelcraft_skill_hunting_progress_percent%
```

These require the optional PlaceholderAPI integration. See [Placeholder reference](../../reference/placeholders.md).

---

[← Documentation contents](../../README.md) · [Project homepage](../../../README.md)
