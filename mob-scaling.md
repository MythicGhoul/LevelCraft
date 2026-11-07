# Mob difficulty & scaling

LevelCraft levels ordinary mobs to remain relevant as players progress. A recent balancing update aimed to make early-game mobs less punishing and bring more serious challenges **after Total Level 150**.

## Current documented tuning

A November 2026 `config(10).yml` reference contains the following values:

```yaml
Mob-Scaling:
  Enabled: true
  Max-Lvl: 550
  Spawn-Range:
    Min-Factor: 0.90
    Max-Factor: 1.10
  Progression:
    Enabled: true
    Challenge-Starts-At: 150
    Health:
      Early-Per-Level: 0.015
      Late-Quadratic: 0.000095
      Max-Multiplier: 25.0
    Damage:
      Early-Per-Level: 0.006
      Late-Quadratic: 0.000030
```

This is an **extract of a project configuration**, not a replacement `config.yml`. Keep the remaining settings from your generated config.

## How the curve behaves

The comment in that config describes the general multiplier:

```text
multiplier = min(cap,
    1 + mobLevel × earlyRate
      + max(0, mobLevel − 150)² × lateRate)
```

The health and damage parameters use their respective rates. This produces gradual growth below level 150 and accelerated scaling above it, subject to configured caps.

## Which player determines mob level?

The referenced configuration states that normal mobs track the **lowest nearby player's Total Level** rather than distance from world spawn. This keeps mixed-level groups more playable. Older `Distance-Lvl-Up` configuration keys may remain for backward compatibility but are not active in this newer player-relative mode.

## Exceptions

Bosses and certain exceptional entities (such as Wardens, Withers, Ender Dragons and corruption guardians) are excluded from this ordinary-mob curve. Read [Bosses](bosses.md) and [Corruption](corruption.md) for their separate balancing.

## Diagnostics

When a level-10 player meets an unexpectedly powerful mob, check nearby high-level players, stale metadata on already-spawned mobs, a special-entity exception, world encounters and other plugins that modify attributes.
