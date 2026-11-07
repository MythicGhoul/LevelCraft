# Extending LevelCraft safely

LevelCraft offers several integration points through Bukkit events, persistent item metadata, the Vault API, PlaceholderAPI and world map hooks. The correct implementation depends on the actual source version.

## Before editing code

1. Work from a copy of the **current** installed plugin source.
2. Identify the relevant manager and event listeners.
3. Decide whether your new logic belongs at XP award, item creation, inventory transaction, player profile loading or world update time.
4. Check existing cancel and duplication-prevention logic.
5. Add tests that reproduce the specific problem before changing the implementation.

## Adding an XP source

Route the award through the common XP manager and its multiplier checks rather than directly setting an XP amount. This preserves global events, prestige bonuses, action-bar feedback and other shared rules.

## Adding a custom item

Use a stable namespaced identifier in persistent item data, plus readable lore and a valid material. Keep creation, recognition and ability handling in separate functions where possible. Give item GUIs and third-party integrations the complete `ItemStack` metadata.

## Adding a world feature

Persist the world UUID/location and state so entities and markers can be rebuilt after restart. Keep chunk loading bounded, handle world unload events and ensure cleanup is idempotent.

## Adding a placeholder

Return a safe string for both online and offline/invalid contexts, and avoid expensive scans for placeholders frequently updated by scoreboards. Prefer cached values when possible.

## Version caution

Do not copy an old code snippet directly into 26.3 without checking updated Bukkit materials, attribute APIs and entity metadata changes.
