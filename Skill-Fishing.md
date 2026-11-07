# Fishing

**Catching fish and developing expertise at water-based gathering.**

## How to earn Fishing XP

Catch fish through valid rod casts and participate in fishing events.

Every XP source has eligibility checks, and award amounts may vary by material, entity, action, environment and the installed build. Use the character sheet to confirm a real increase rather than relying only on the action-bar animation.

## Milestones and rewards

Weight-based XP and fishing-specific bonuses or competitions. See [Skill milestones](https://github.com/MythicGhoul/LevelCraft/wiki/Milestones) for the common level-10, level-25, level-40 and level-50 framework. The actual perk names, odds and values come from the currently installed code and YAML.

## Practical tips

- Train through normal survival activities instead of farming a single low-value action indefinitely.
- Check [Total Level](https://github.com/MythicGhoul/LevelCraft/wiki/Total-Level-and-XP) as the skill improves; Total Level affects broader combat and item effectiveness.
- Look for [Quest](https://github.com/MythicGhoul/LevelCraft/wiki/Quests) steps involving this activity, which may award extra skill XP.
- Some world events and prestige benefits modify eligible XP awards.

## Detailed Fishing mechanics

### Fish weight
Fishing experience is designed to reflect fish weight or value, making rare/heavier catches more meaningful than identical flat rewards. Rod quality and item rarity can affect the expected fishing experience.

### Events and challenges
Fishing competitions can track how many catches a player lands, and their timer may be visible on a scoreboard. Use the event's rules to decide whether you are optimising total catches, weight or another objective.

## Known interactions

Fishing XP can scale with fish weight; the catch and event configurations control results.

## Checking a scoreboard value

```text
%levelcraft_skill_fishing_level%
%levelcraft_skill_fishing_xp%
%levelcraft_skill_fishing_xp_required%
%levelcraft_skill_fishing_progress_percent%
```

These require the optional PlaceholderAPI integration. See [Placeholder reference](https://github.com/MythicGhoul/LevelCraft/wiki/Reference-Placeholders).

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Progression](https://github.com/MythicGhoul/LevelCraft/wiki/Character-Progression) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
