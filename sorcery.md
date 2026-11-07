# Sorcery

**Casting and learning magic through mana-driven spell progression.**

## How to earn Sorcery XP

Learn spells from tomes and cast valid spells using wands or other configured equipment.

Every XP source has eligibility checks, and award amounts may vary by material, entity, action, environment and the installed build. Use the character sheet to confirm a real increase rather than relying only on the action-bar animation.

## Milestones and rewards

Increasing mana capacity, regeneration and magical combat options. See [Skill milestones](../milestones.md) for the common level-10, level-25, level-40 and level-50 framework. The actual perk names, odds and values come from the currently installed code and YAML.

## Practical tips

- Train through normal survival activities instead of farming a single low-value action indefinitely.
- Check [Total Level](../leveling.md) as the skill improves; Total Level affects broader combat and item effectiveness.
- Look for [Quest](../../quests/overview.md) steps involving this activity, which may award extra skill XP.
- Some world events and prestige benefits modify eligible XP awards.

## Detailed Sorcery mechanics

### Spell learning and casting
A player can know a spell without meeting its usage requirements. Sorcery progression, mana capacity, available wands, spellbook loadout and cooldowns all affect what can be cast.

### Training and balancing
The school or tier of a spell may influence XP and damage. Test cheap healing, single-target attacks and high-cost area spells separately, and confirm that protected terrain is not unintentionally destroyed by AoE spells.

## Known interactions

Mana costs, cooldowns, spell unlocks and spellbook selection all interact.

## Checking a scoreboard value

```text
%levelcraft_skill_sorcery_level%
%levelcraft_skill_sorcery_xp%
%levelcraft_skill_sorcery_xp_required%
%levelcraft_skill_sorcery_progress_percent%
```

These require the optional PlaceholderAPI integration. See [Placeholder reference](../../reference/placeholders.md).
