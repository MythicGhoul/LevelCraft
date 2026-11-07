# Coins and currency rewards

Coins provide a spendable progression resource. They can originate from creature drops, quest rewards, selling items or special encounters, depending on the configured systems.

## Coin features

- Custom coin drops and pickup feedback.
- Configurable coin bag behaviour and merging.
- NPC purchasing, selling and guild-buyer exchanges.
- Quest rewards and cost requirements through Vault.
- Economy values in the character UI and PlaceholderAPI (`%levelcraft_money%`).

## Economy checklist

1. Confirm Vault and an economy provider both start successfully.
2. Check that a player can receive money through a valid action.
3. Test buying and selling in an NPC shop.
4. Check a quest cost/reward with a low-balance test account.
5. Review logs for failed transactions and duplicate rewards.

## Security and balancing

Do not trust client-visible item names or transaction GUI text as the source of truth for balance changes. Item costs and item delivery should be validated server-side. For bulk purchases, deduct the intended total before or atomically with item delivery.
