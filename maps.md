# Dynmap and BlueMap

LevelCraft has integration points for **Dynmap** and **BlueMap**, allowing progression systems to be visible on web maps.

## Supported map concepts

| Data | Example presentation |
| --- | --- |
| Corruption | Area polygons, core level, guardian status |
| Shrines | Structure markers and active status |
| NPC markets | Shop or town markers |
| Clans | Territory outlines and claimed regions |
| Boss spawners | Arena or spawn point markers |

Actual marker availability depends on which hooks are enabled by your build and which data managers initialise successfully.

## Setup

1. Install the map plugin that matches your server.
2. Enable its integration and check the startup log for hook registration.
3. Create a shrine, core, NPC shop or claim to supply something to display.
4. Restart if your build only registers existing markers on startup.
5. Inspect the web map layers/marker sets and test a new update.

## Missing marker checklist

Check world identifiers, marker set visibility, configured integrations, plugin startup ordering, database/state loading and whether the map plugin has finished rendering. If one map works but the other does not, focus on the specific adapter and supported API version.

**Privacy:** publish only the map layers you want players to see. Exposing all clan borders or unrevealed shrines can change your server's intended exploration experience.

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
