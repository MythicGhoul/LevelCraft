# Custom bosses & spawners

Bosses are deliberate high-difficulty encounters. They can support guild promotion exams, corruption events or dedicated arenas, and they follow their own balancing rather than the gentler normal-mob curve.

## Features

- Custom health, damage, appearance and arena design.
- Nearby boss bars and encounter visibility.
- Death title/subtitle events and return-to-arena workflows.
- Configurable loot/reward sets and optional command rewards.
- Persistent boss spawners at configured locations.

## Spawner administration

Referenced development includes a boss-spawner command family with actions analogous to `create`, `remove`, `list`, `tp`, `reload` and `addstart` under `/lc admin spawner`. These subcommands must be checked against the deployed build's command router before use.

## Design an encounter

1. Create a controlled arena with safe player entry and exit points.
2. Configure the boss data and difficulty.
3. Attach the boss to its spawner or exam.
4. Test death, respawn/return, rewards, party participation and repeated activation.
5. Add web-map markers only if you want the location publicly discoverable.

## Performance

Limit simultaneously active bosses and expensive particle patterns. Keep area-of-effect checks within a bounded radius, and avoid spawning heavy entities for idle or unloaded arenas.

See [Promotion exams](https://github.com/MythicGhoul/LevelCraft/wiki/Promotion-Exams) and [Mob scaling](https://github.com/MythicGhoul/LevelCraft/wiki/World-Mob-Scaling).

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 World](https://github.com/MythicGhoul/LevelCraft/wiki/World-Systems) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
