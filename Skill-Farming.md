# Farming

**Growing crops, harvesting produce and raising animals.**

## How to earn Farming XP

Harvest valid crop stages, replant fields and breed eligible animals.

Every XP source has eligibility checks, and award amounts may vary by material, entity, action, environment and the installed build. Use the character sheet to confirm a real increase rather than relying only on the action-bar animation.

## Milestones and rewards

Improved harvesting, farming quality-of-life and agricultural milestones. See [Skill milestones](https://github.com/MythicGhoul/LevelCraft/wiki/Milestones) for the common level-10, level-25, level-40 and level-50 framework. The actual perk names, odds and values come from the currently installed code and YAML.

## Practical tips

- Train through normal survival activities instead of farming a single low-value action indefinitely.
- Check [Total Level](https://github.com/MythicGhoul/LevelCraft/wiki/Total-Level-and-XP) as the skill improves; Total Level affects broader combat and item effectiveness.
- Look for [Quest](https://github.com/MythicGhoul/LevelCraft/wiki/Quests) steps involving this activity, which may award extra skill XP.
- Some world events and prestige benefits modify eligible XP awards.

## Detailed Farming mechanics

### Harvesting
Farming can reward mature crop harvests and breeding. Earlier XP tuning included plant-growth logic that credits farming after a valid harvest rather than when the crop is first planted.

### What to test
Plant, harvest mature, break immature and replant the same crop. Compare the XP awards. Then test breeding separately, since animal husbandry is not the same event as crop harvesting.

## Known interactions

Immature crop breaks may not award XP. Harvest and breed conditions are server-controlled.

## Checking a scoreboard value

```text
%levelcraft_skill_farming_level%
%levelcraft_skill_farming_xp%
%levelcraft_skill_farming_xp_required%
%levelcraft_skill_farming_progress_percent%
```

These require the optional PlaceholderAPI integration. See [Placeholder reference](https://github.com/MythicGhoul/LevelCraft/wiki/Reference-Placeholders).

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Progression](https://github.com/MythicGhoul/LevelCraft/wiki/Character-Progression) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
