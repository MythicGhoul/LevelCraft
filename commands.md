# Commands reference

This page separates commands **seen in the referenced `plugin.yml` or `LevelCraftCommand` source** from subcommands described during development but not independently verified in the latest build.

## Core player commands

| Command | Purpose | Source confidence |
| --- | --- | --- |
| `/lc` or `/levelcraft` | LevelCraft main menu / help | Registered |
| `/lc stats` | Character stats GUI | Confirmed in handler |
| `/stats` or `/profile` | Open character stats | Registered |
| `/lc top` | Top players leaderboard | Confirmed in handler |
| `/lc forge` | Open the forge | Confirmed in handler |
| `/lc sockets` | Open sockets interface | Confirmed in handler |
| `/lc guide` | Open guide | Confirmed in handler |
| `/lc prestige` | Prestige interface | Confirmed in handler |
| `/lc quests` | Quest interface | Confirmed in handler |
| `/quests`, `/quest`, `/q` | Quest interface aliases | Registered |
| `/lc rank` | Rank/path GUI | Confirmed in handler |
| `/lc rank info` | Character rank information | Confirmed in handler |
| `/party` or `/p` | Party commands | Registered |
| `/clan` | Clan commands | Registered |
| `/lc quests active` | List active quests | Documented in handler |
| `/lc quests claim <quest>` | Claim a ready quest | Documented in handler |
| `/spells` or `/spellbook` | Aliases of main `/lc` dispatcher | Registered (behaviour handled in code) |

!!! info "Aliases and version differences"
    A registered command alias can route to a specific menu even when its `plugin.yml` entry points to `/lc`. For example, Sorcery aliases may open the spellbook on current builds. Use the installed version's help output as the definitive behaviour.

## Confirmed administration commands

These syntax lines appear in the referenced LevelCraft command source:

```text
/lc admin
/lc admin reload
/lc admin shrine spawn
/lc admin starterkit <player>
/lc admin pathsign <path>
/lc admin pathsign remove <path>
/lc admin pathsign list
/lc admin pathsign cancel
/lc admin pathsign reload
/lc admin mana <player> <set|add|remove> <amount>
/lc admin quests editor
/lc admin quests reload
/lc admin quests give <player> <quest>
/lc admin quests remove <player> <quest>
/lc admin quests reset <player>
/lc admin souls <player> <amount>
/lc admin addlevel <player> <skill|all> <amount>
/lc admin misc list
/lc admin misc <item> [player] [amount]
/lc admin furnace list
/lc admin furnace <player> <tier/all> [amount]
/lc admin scale <player> <scale>
/lc admin scale reset <player>
/lc admin discordtest
```

Use `/lc admin` to access the admin GUI when enabled; administrative subcommands require appropriate elevated permissions. `pathsign` setup can be location-sensitive and should be performed by a player in the world rather than blindly through console.

## Additional systems with separate routers

- **Corruption:** `/lc admin corruption ...` delegates to a corruption command handler; consult its current help.
- **Boss spawners:** development included `/lc admin spawner` management subcommands; verify before use.
- **Villager shops:** referenced NPC data points to `/lc admin villager` or the in-game admin GUI.
- **Player trading:** `/trade <player>` is a separately registered workflow in builds where it is installed.
- **Random teleport:** `/rtp` was added as an optional server movement command in recent builds.

## When a command does nothing

Check whether it is listed by `/help`, whether the implementation is registered in the correct JAR, whether the sender is a player or console, and whether permissions or another plugin intercepted it. See [Troubleshooting](../administration/troubleshooting.md).
