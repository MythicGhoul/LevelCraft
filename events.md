# Global and timed events

World events give players time-limited reasons to explore, fight and compete. The documented LevelCraft ecosystem includes several distinct event types.

## Double XP

A global XP event applies a multiplier to eligible skill awards. Its status can be exposed through `%levelcraft_xp_event_active%`, `%levelcraft_xp_event_multiplier%` and `%levelcraft_xp_event_remaining%`.

> **Testing a multiplier**
>
> Compare the same eligible action under normal conditions and while the event is active. If a 2× event still grants only the base amount, verify that the multiplier is applied at the final award point, not only to GUI display messages.


## Blood Moon

The `Blood-Moon` configuration can alter night-time threats and spawn pressure. The referenced project config includes zombie count controls. Servers should tune this carefully to prevent crowding a spawn or low-power settlement.

## Fishing events

Fishing events track catches and optional competitions. PlaceholderAPI reports whether an event is active, the time remaining and a player's catch count.

## Hive and corruption storms

Corruption systems can trigger server-wide threats or themed storms. Administrators previously rebalanced their frequency to avoid excessive disruption. These are especially suitable for Discord announcements and map overlays.

## Event setup checklist

Set a maximum number of affected mobs, schedule appropriate downtime between events, exclude protected areas and verify that rewards cannot be repeatedly claimed through relogging or region hopping.

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
