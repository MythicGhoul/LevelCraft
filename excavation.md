# Excavation

**Excavating dirt, sand, gravel and other diggable blocks.**

## How to earn Excavation XP

Dig eligible terrain using proper tools and pursue excavation quests.

Every XP source has eligibility checks, and award amounts may vary by material, entity, action, environment and the installed build. Use the character sheet to confirm a real increase rather than relying only on the action-bar animation.

## Milestones and rewards

More valuable and efficient digging rewards. See [Skill milestones](../milestones.md) for the common level-10, level-25, level-40 and level-50 framework. The actual perk names, odds and values come from the currently installed code and YAML.

## Practical tips

- Train through normal survival activities instead of farming a single low-value action indefinitely.
- Check [Total Level](../leveling.md) as the skill improves; Total Level affects broader combat and item effectiveness.
- Look for [Quest](../../quests/overview.md) steps involving this activity, which may award extra skill XP.
- Some world events and prestige benefits modify eligible XP awards.

## Detailed Excavation mechanics

### Eligible digging
Excavation is most naturally progressed through sand, gravel, dirt and other earth materials. Its XP should be distinct from Mining, even when both use block break events.

### Anti-farm logic
A practical implementation checks protected/spawn areas and whether the action genuinely represents gathering. If players can repeatedly place and dig the same block for full XP, admins should review the server's chosen anti-farm rules.

## Known interactions

XP is usually awarded on permitted block breaks, subject to anti-farm protections.

## Checking a scoreboard value

```text
%levelcraft_skill_excavation_level%
%levelcraft_skill_excavation_xp%
%levelcraft_skill_excavation_xp_required%
%levelcraft_skill_excavation_progress_percent%
```

These require the optional PlaceholderAPI integration. See [Placeholder reference](../../reference/placeholders.md).
