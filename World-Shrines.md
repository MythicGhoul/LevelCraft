# World shrines & structure loot

Shrines are procedurally placed structures that reward players for exploring and investigating the world. Depending on the build, they can be generated near exploration activity or by scheduled/world-driven spawning independent of players.

## Finding a shrine

Search distant terrain, use clues or consult configured BlueMap/Dynmap markers if your server exposes them. Administrators can adjust minimum distances, eligible biomes, placement attempts and structure schematics.

## Typical shrine flow

1. Locate an active shrine.
2. Explore and interact with its structure and loot.
3. Claim eligible rewards.
4. Observe the deconstruction or collapse effect when its active phase ends.
5. Allow the world cleanup system to finish before rebuilding within the affected area.

The collapse system uses effects such as crumbling blocks, particles and sound to make the structure feel temporary rather than simply disappearing in one tick.

## Loot conversion

Loot chests and vanilla structures may contain unconverted weapons, armour and tools. Recent LevelCraft development added structure-loot conversion so eligible vanilla gear becomes recognised LevelCraft equipment. This helps preserve rarity and Power Level progression across exploration content.

## Admin operation

A referenced command handler supports `/lc admin shrine spawn` to generate a test shrine near the executing player. Use it on staging and validate terrain, schematic placement, loot, state saves and collapse cleanup.

> **World editing**
>
> Schematic placement and destructive collapse affect world blocks. Keep backups and test protection-plugin interactions. Optional WorldEdit/FAWE integration is build-dependent.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 World](https://github.com/MythicGhoul/LevelCraft/wiki/World-Systems) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
