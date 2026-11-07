# Exploration

**Travelling, discovering new places and surviving unfamiliar terrain.**

## How to earn Exploration XP

Move through the world, discover new biomes and use valid movement activities.

Every XP source has eligibility checks, and award amounts may vary by material, entity, action, environment and the installed build. Use the character sheet to confirm a real increase rather than relying only on the action-bar animation.

## Milestones and rewards

Travel-oriented rewards and progression for active adventurers. See [Skill milestones](../milestones.md) for the common level-10, level-25, level-40 and level-50 framework. The actual perk names, odds and values come from the currently installed code and YAML.

## Practical tips

- Train through normal survival activities instead of farming a single low-value action indefinitely.
- Check [Total Level](../leveling.md) as the skill improves; Total Level affects broader combat and item effectiveness.
- Look for [Quest](../../quests/overview.md) steps involving this activity, which may award extra skill XP.
- Some world events and prestige benefits modify eligible XP awards.

## Detailed Exploration mechanics

### Discovery and movement
Exploration can reward new biome discoveries and eligible movement actions, including some vehicle/travel and fall-related interactions in earlier builds. It should encourage travel rather than repeatedly triggering a stationary action.

### Random rewards
Previous iterations included random item drops or occasional bonus effects during exploration. Later design work moved away from disruptive random litter; actual abilities should be checked on your deployed build.

## Known interactions

Recent design work replaced or revised random dropped rewards; exact exploration abilities depend on the current build.

## Checking a scoreboard value

```text
%levelcraft_skill_exploration_level%
%levelcraft_skill_exploration_xp%
%levelcraft_skill_exploration_xp_required%
%levelcraft_skill_exploration_progress_percent%
```

These require the optional PlaceholderAPI integration. See [Placeholder reference](../../reference/placeholders.md).

---

[← Documentation contents](../../README.md) · [Project homepage](../../../README.md)
