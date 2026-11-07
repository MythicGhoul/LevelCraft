# Direct player trading

The player trade system is designed for **item-for-item exchange** with no mandatory coin payment.

## Proposed flow used in development

1. Player A sends `/trade <player>`.
2. Player B receives an invitation and chooses Accept or Deny.
3. Both players open a linked trade window.
4. Each adds their own offered items to their side of the interface.
5. Both players must independently confirm the offer.
6. After final confirmation, the items are exchanged safely.

## Essential safety properties

- Neither player may remove another player's offered items.
- Offer changes reset any previous confirmation.
- Closing or cancelling returns every offered item to its original owner.
- Full inventories, disconnects and server shutdowns are handled without losing or duplicating items.
- Third-party custom items must be transferred with their complete `ItemMeta` and persistent data.

> **Availability**
>
> A standalone `/trade` implementation was being added and debugged in earlier project work. The exact command registration and release status must be checked on the live server, rather than treating this workflow as proof that the command is enabled everywhere.

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
