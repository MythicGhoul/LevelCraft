# Troubleshooting

Use this checklist to isolate problems without risking production data. Test with a plain player account, an eligible vanilla item and a normal survival world before investigating complex plugin interactions.

## A command shows its usage and nothing happens

Check `plugin.yml` registration, actual command executor registration in the running JAR, permissions and whether the feature's manager loaded. This was a particular concern when adding standalone `/trade` and other separate command handlers.

## Double XP does not change awards

Compare the XP awarded by the same eligible action before and during a 2× event. If both awards are unchanged, inspect where the XP multiplier is applied in the award pipeline. The action-bar display may update independently of the real XP balance. Make sure a second handler has not directly written XP and bypassed event multipliers.

## Unexpectedly strong early-game mobs

Confirm the installed `Mob-Scaling.Progression.Challenge-Starts-At` and its early/late multipliers. Rule out bosses, corruption guardians, already-spawned mobs and high-level players nearby. The gentler November tuning aims for harder difficulty only beyond level 150.

## A quest does not progress

Verify that its `Type`, `Target`, `Amount`, guild tier and questline prerequisites match the actual event. A handler using `MINE_BLOCK` will not necessarily recognise a made-up enum string or a block broken through a protection plugin.

## Vanilla loot does not have LevelCraft rarity

Confirm that loot conversion listeners cover the structure generation/loot event used by that container. Loot from external plugins and already-filled containers may need separate handling.

## Spell will not cast

Check that the spell is known and usable, the wand has real LevelCraft metadata, the selected loadout is valid, sufficient mana exists and no cooldown is active. Also check click interception by protection or inventory plugins.

## Custom nametags disappear

Look for conflicts with scoreboard teams, tab-list plugins and nametag overrides. Verify that both observer and target player have their tags updated, and that floating text is cleaned up on quit.

## BlueMap or Dynmap markers are missing

Verify plugin installation, integration startup logs, world IDs, marker visibility, valid manager data and startup order. For some builds, restarting after creating the first shrine or NPC refreshes marker initialisation.

## Items show black/purple missing textures

Check whether the resource pack downloaded; test manual installation, pack format, item model definitions, namespaced texture paths and the SHA-1. A pack that works locally but fails on join often points to hosting URL, response headers or hash problems.

## Duplicate starter kit

Inspect join/character-creation events. A kit must be granted exactly once for an eligible new character. Restore player-kit markers carefully if data has been wiped; do not simply grant on every login.

## Config silently reverts

Check YAML syntax, updater/migration logs and backup folder contents. Some settings are regenerated or migrated when a plugin detects an old config version.

## Server performance declines

Check encounter caps, corruption chunks, shrine collapse batches, high-frequency particles and nametag tick updates. Measure server MSPT separately from client FPS.

## Last resort: minimal reproduction

Copy the server to staging, disable nonrequired integrations, reproduce with one test account, collect a precise stack trace and re-enable other plugins one at a time. Never remove a production player's `.yml` data to “test” a fix without first saving it.
