# Woodcutting

**Harvesting trees and gathering sustainable wood resources.**

## How to earn Woodcutting XP

Break eligible log blocks; manage forests; use the Tree Feller ability where unlocked.

Every XP source has eligibility checks, and award amounts may vary by material, entity, action, environment and the installed build. Use the character sheet to confirm a real increase rather than relying only on the action-bar animation.

## Milestones and rewards

Faster timber collection and specialised tree-harvesting perks. See [Skill milestones](../milestones.md) for the common level-10, level-25, level-40 and level-50 framework. The actual perk names, odds and values come from the currently installed code and YAML.

## Practical tips

- Train through normal survival activities instead of farming a single low-value action indefinitely.
- Check [Total Level](../leveling.md) as the skill improves; Total Level affects broader combat and item effectiveness.
- Look for [Quest](../../quests/overview.md) steps involving this activity, which may award extra skill XP.
- Some world events and prestige benefits modify eligible XP awards.

## Detailed Woodcutting mechanics

### Tree Feller
Tree Feller can turn an ordinary tree-cutting session into an efficient mass harvest after the appropriate milestone. Because one click can remove many logs, the plugin must distinguish eligible natural blocks and guard against protected areas.

### XP expectations
Log type and number of actually removed blocks matter. A multi-block ability should not accidentally count the triggering log twice or award XP from unrelated adjacent builds.

## Known interactions

Tree Feller and related mechanics may have cooldowns and block-protection rules.

## Checking a scoreboard value

```text
%levelcraft_skill_woodcutting_level%
%levelcraft_skill_woodcutting_xp%
%levelcraft_skill_woodcutting_xp_required%
%levelcraft_skill_woodcutting_progress_percent%
```

These require the optional PlaceholderAPI integration. See [Placeholder reference](../../reference/placeholders.md).
