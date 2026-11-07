# Socket gems

Sockets provide custom item modifiers through a specialised gem system. Each gem has a type/category, tier and effect, and only compatible item classes should accept it.

## Gem tiers

LevelCraft development tracks **Tier I, Tier II and Tier III** gems. Higher tiers can offer greater modifiers. Balancing of stacking multiple high-tier gems has been revised, so the numerical bonus must be read from the installed system rather than assumed from old values.

## How to use sockets

1. Acquire or craft a compatible gem.
2. Open the socket interface with `/lc sockets` (or the configured admin/player GUI).
3. Select eligible gear containing a socket.
4. Choose the gem and read the preview.
5. Apply the gem or remove it using the permitted removal workflow.

## Restrictions

- Item category restrictions prevent arbitrary stacking (for example, a weapon gem should not automatically fit an unrelated fishing rod).
- Each item has a finite socket capacity.
- Gems and socket counts are stored in persistent item data; do not create them by altering lore text alone.
- The removal permission `lc.sockets` is listed as a player-default permission in the referenced manifest.

Placeholders such as `%levelcraft_held_item_sockets%` and `%levelcraft_held_item_gems%` support HUD integration.

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
