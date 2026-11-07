# Levels, XP & Total Level

Each skill has its own XP pool and level. Performing a valid activity awards XP to the related skill. The action bar and character menus communicate progression, while milestone levels award special improvements.

## Skill XP

The publicly described progression curve for LevelCraft is approximately `50 × level^1.5`; exact rounding, XP multipliers and version-specific curves depend on the installed code and config. This is a **skill XP curve**, not a claim that every block or enemy pays the same amount.

A mining action may earn only a small amount of Mining XP, while an important ore, boss or quest reward can award more. Global XP events and prestige bonuses can modify awarded amounts.

## Total Level

Recent LevelCraft work rebalanced Total Level as percentage-based character progress. Key design targets are:

- A fresh character with each skill beginning at level 1 reports **Total Level 1**, not 11.
- Total Level tracks overall mastery and is designed for a **maximum of 550**.
- Equipment Power Level and normal mob scaling compare against Total Level.
- Individual skill levels remain independently meaningful for abilities and milestones.

Do not add your eleven skill levels together and expect that number to match the character sheet.

## XP multipliers and events

XP may be adjusted by global double-XP events, prestige rewards, skill effects or party sharing. If a supposed `2×` event still displays an unchanged reward, check [XP troubleshooting](https://github.com/MythicGhoul/LevelCraft/wiki/Admin-Troubleshooting#double-xp-does-not-change-awards) rather than assuming the display is correct.

## Common reasons XP is denied

Server-controlled reasons can include spawn protection, activity restrictions, already-placed blocks or actions that are not valid XP sources. Recent LevelCraft setups have used a **125-block spawn exclusion** for some XP farming. Check the installed configuration and listeners for the exact scope.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Progression](https://github.com/MythicGhoul/LevelCraft/wiki/Character-Progression) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
