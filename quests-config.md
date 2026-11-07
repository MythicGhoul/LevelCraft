# Quest YAML reference

Quest definitions live under the `Quests:` root in a referenced `quests.yml`. The following is adapted from an actual early quest entry in LevelCraft project data; it uses the same key structure and a standard vanilla target.

```yaml
Quests:
  woodsman:
    Display-Name: '&6Woodcutting Skill'
    Type: CHOP_LOG
    Target: OAK_LOG
    Amount: 10
    Quest-Line: starter
    Line-Order: 1
    Permission-Tier: F
    Repeatable: false
    Rewards:
      Economy:
        Enabled: false
        Amount: 0
      Skill-XP:
        Enabled: true
        Rewards:
          WOODCUTTING: 50
      Items:
        Enabled: false
        Rewards: []
      Commands:
        Enabled: false
        Rewards: []
```

## Fields explained

| Key | Meaning |
| --- | --- |
| Quest ID (`woodsman`) | Unique machine ID used in saved progression. |
| `Display-Name` | Colour-formatted player-facing title. |
| `Type` | Objective handler (e.g. `CHOP_LOG` or `MINE_BLOCK`). |
| `Target` | Required block, mob, recipe or spell reference, depending on type. |
| `Amount` | Quantity to complete. |
| `Quest-Line` | Group of ordered quests. |
| `Line-Order` | Step position inside the group. |
| `Permission-Tier` | Eligible guild rank, typically F through S. |
| `Repeatable` | Whether the quest can be re-completed. |
| `Rewards.Economy` | Vault-linked currency rewards. |
| `Rewards.Skill-XP` | Per-skill XP rewards. |
| `Rewards.Items` | Configured item rewards. |
| `Rewards.Commands` | Command rewards. |

## Adding a quest

Choose a new ID, copy the structure from a *working quest in your installed file*, update the type and target, and assign an unused ordering slot in the appropriate questline. Validate with `/lc admin quests reload` when supported, then test acceptance, tracking, claim and reward delivery.

## Promotion and voting objectives

Promotion exams may use separate quest definitions or special steps. Optional vote and economy cost objectives require their corresponding integrations to be enabled. Do not assume custom objective enum spelling: inspect the live quest editor or parser when implementing an unfamiliar quest type.

## Failure scenarios to test

- Two quests with the same ID or line order.
- Invalid material or entity names.
- Completion after a player disconnects or changes worlds.
- Repeated reward claiming.
- Missing economy provider.
- Invalid console commands or plugin-specific item serialization.

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
