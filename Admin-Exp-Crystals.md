# Configuring EXP crystals

EXP crystals are special consumables awarded through eligible ore drops. Their appearance can be customised by a resource pack, and each crystal carries its associated skill as persistent item data.

## Design

- Underlying item material: **`AMETHYST_SHARD`** in the referenced implementation.
- Each crystal is assigned a skill from the LevelCraft skill list.
- Admins can set a drop chance from 0–100%, along with minimum and maximum XP granted.
- The displayed lore shows the skill, XP range and usage directions.
- A texture pack can supply distinct crystal art per skill.

## Configuring drop chance

If the config defines chance in the range 0–100, a value of `100.0` is an always-drop test configuration. Do not confuse a chance expressed as a percentage with a probability expressed as 0–1; read the generated config comments.

## Testing

1. Temporarily set the desired ore drop chance to 100 on a test server.
2. Break an eligible naturally generated ore.
3. Confirm the crystal has its proper name, lore and enchant glow.
4. Right-click to consume it and inspect the relevant skill's XP.
5. Repeat with placed ores and Fortune/Silk Touch to evaluate the current block-handling logic.
6. Restore the real drop chance before reopening the server.

## Resource pack problems

Black-and-purple items usually mean the selected custom texture is missing, misnamed or incompatible with the server's item components/model format. Check the pack structure, version and SHA-1, then confirm it loads manually before troubleshooting automatic download.

## Reloads

Recent builds intended `/lc admin reload` to reload the specialised EXP crystal YAML. Test this on your version: some settings may still require a restart.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Administration](https://github.com/MythicGhoul/LevelCraft/wiki/Administration) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
