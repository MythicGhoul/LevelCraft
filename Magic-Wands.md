# Wands & spell controls

Wands determine how a player casts spells. Different wand tiers support different power levels and spell compatibility.

| Wand | Referenced base item | Role |
| --- | --- | --- |
| Lesser Wand | Stick | Early spellcasting |
| Greater Wand | Blaze rod | More advanced sorcery |
| Meteor Wand | Fire charge | High-tier AoE magic |

These are the base Minecraft materials used for identification in a referenced implementation; official LevelCraft item metadata distinguishes a wand from an ordinary stick, blaze rod or fire charge.

## Using a wand

1. Learn a spell through its tome or a valid unlock.
2. Equip a compatible wand.
3. Select a usable spell from the wand rotation or spellbook.
4. Cast with the configured attack interaction and wait for its cooldown.
5. Keep enough mana available for the next cast.

## Problems to check

- A non-LevelCraft item has the right material but lacks metadata.
- The spell is learned but not available to the held wand.
- Cooldown is still running.
- Mana is insufficient.
- The selected combat loadout has empty slots.
- Another plugin cancels the click or prevents combat at the target location.

See [Magic troubleshooting](https://github.com/MythicGhoul/LevelCraft/wiki/Admin-Troubleshooting).

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Magic](https://github.com/MythicGhoul/LevelCraft/wiki/Magic) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
