# Nametags & overhead information

The custom nametag system displays character identity and combat status in the world. A recent design uses guild rank beside the player's name, with floating level and health information positioned above or below the main nameplate.

## Display concepts

- Guild rank shown near the player name.
- Total Level and health displayed in a separate hologram/text line.
- Health colour transitions from **green → yellow → orange → red** as health falls.
- Text offset and following logic to stay aligned with moving players.

## Compatibility

Other plugins that control scoreboard teams or player display names can interfere with tag ordering. MythicTab and SimpleScore-like features should be checked when names lose their rank text.

## Troubleshooting

If one player sees the custom label while another does not, inspect scoreboard team ownership for both clients, plugin priority, nametag update events and entity cleanup on quit/reload. Floating text should be removed cleanly to avoid static labels remaining in unloaded areas.

See [Troubleshooting](../administration/troubleshooting.md) and [Placeholders](../reference/placeholders.md).
