# Spell catalogue & learning

LevelCraft's magic toolkit includes healing, elemental attacks, area effects and higher-tier spells. Availability is based on tomes, unlocks, Sorcery level and the configured spell registry.

## Documented spell families

| Family | Examples | Purpose |
| --- | --- | --- |
| Healing | Healing, Greater Healing | Restore health and support survival |
| Fire | Flame, Greater Flame | Damage and fire effects |
| Lightning | Lightning, Greater Lightning | Targeted electrical attacks |
| Ice | Ice, Greater Ice | Damage and crowd control |
| Meteor | Meteor | High-tier area attack |
| Additional schools | Poison, Earth, Wind, Life Steal, Void | Expanded utility and damage concepts |
| Legendary concepts | Event Horizon, Heaven's Judgement | Endgame spell designs |

> **Version-dependent catalogue**
>
> Earlier conversations included both implemented spells and later requested additions. This page records the documented families, **not a guarantee that every named spell is available in every released JAR**. The live spellbook and `SpellRegistry` are authoritative.


## Learning spells

A spell tome teaches the corresponding spell through the discovery manager. Known spells are not necessarily usable: restrictions such as required Sorcery level, compatible wand and loadout availability may apply.

## Spellbook

The spellbook offers an interface to inspect learned spells, group them by class/type and assign them to a quick-use loadout. In the six-slot implementation, the player chooses which six spells are convenient to cast during an encounter.

## Balancing

Spells can have separate damage, cooldown, range, mana cost and area settings. AoE spells such as Meteor are designed to affect entities without directly damaging the world terrain in the referenced implementation.

See [Wands](wands.md) and [Mana](mana.md).

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
