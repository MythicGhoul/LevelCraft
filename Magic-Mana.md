# Mana, cooldowns and regeneration

Mana is the resource used to cast LevelCraft spells. Maximum mana, regeneration and spell cooldowns limit repeated ability use and make Sorcery progression valuable.

## Mechanics

- **Current mana** is spent when a valid spell is cast.
- **Maximum mana** determines the size of the available pool.
- **Mana regeneration** refills mana according to a configured rate and timer.
- **Cooldowns** prevent certain spells from being repeatedly cast, even when mana is available.

The referenced tuning discussed spell cooldowns in the region of 3–8 seconds, but these are balance targets rather than universal values.

## Admin controls

The referenced command handler supports:

```text
/lc admin mana <player> <set|add|remove> <amount>
```

For example, `/lc admin mana Alex add 25` adds 25 mana to an online player. Use `lc.admin` permission and follow the target build's autocomplete/help output.

## Useful placeholders

`%levelcraft_mana%`, `%levelcraft_max_mana%`, `%levelcraft_mana_regen%`, `%levelcraft_mana_display%` and `%levelcraft_mana_percent%` are present in the referenced expansion.

## Configuration

The main configuration includes a `Mana-Settings` section. Preserve the existing indentation and change only the keys actually present in your installed file.

---

[🏠 Wiki Home](https://github.com/MythicGhoul/LevelCraft/wiki/Home) · [📚 Magic](https://github.com/MythicGhoul/LevelCraft/wiki/Magic) · [↗ GitHub repository](https://github.com/MythicGhoul/LevelCraft)
