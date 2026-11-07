# Combat

**Defeating hostile opponents and developing character combat power.**

## How to earn Combat XP

Defeat eligible mobs; face stronger enemies and bosses; complete combat objectives.

Every XP source has eligibility checks, and award amounts may vary by material, entity, action, environment and the installed build. Use the character sheet to confirm a real increase rather than relying only on the action-bar animation.

## Milestones and rewards

Health and combat-effectiveness growth, weapon synergy and survival-oriented milestones. See [Skill milestones](https://github.com/MythicGhoul/LevelCraft/wiki/Milestones) for the common level-10, level-25, level-40 and level-50 framework. The actual perk names, odds and values come from the currently installed code and YAML.

## Practical tips

- Train through normal survival activities instead of farming a single low-value action indefinitely.
- Check [Total Level](https://github.com/MythicGhoul/LevelCraft/wiki/Total-Level-and-XP) as the skill improves; Total Level affects broader combat and item effectiveness.
- Look for [Quest](https://github.com/MythicGhoul/LevelCraft/wiki/Quests) steps involving this activity, which may award extra skill XP.
- Some world events and prestige benefits modify eligible XP awards.

## Detailed Combat mechanics

### Weapon damage and defence
Combat progression contributes to player fighting power, but a weapon's final effect also depends on rarity, Power Level and the target's defences. A player below a weapon's requirement can be penalised even with a high Combat level. Unarmed combat has a separate bounded scaling model.

### Training safely
Compare equal enemies while changing only one factor: your Combat level, your weapon rarity or the enemy level. This makes it easier to identify whether a balance issue belongs to skill progression, equipment or mob scaling.

## Known interactions

PvP and PvE may award differently. Mob difficulty scales with a player-related level, and the final damage result also depends on Power Level.

## Checking a scoreboard value

```text
%levelcraft_skill_combat_level%
%levelcraft_skill_combat_xp%
%levelcraft_skill_combat_xp_required%
%levelcraft_skill_combat_progress_percent%
```

These require the optional PlaceholderAPI integration. See [Placeholder reference](https://github.com/MythicGhoul/LevelCraft/wiki/Reference-Placeholders).

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Progression](https://github.com/MythicGhoul/LevelCraft/wiki/Character-Progression) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
