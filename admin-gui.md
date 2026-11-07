# In-game editors and admin GUI

Administrative interfaces make it possible to manage complex features without manually writing every YAML entry. In the referenced implementation, the admin controller is opened by `/lc admin` and additional editors are registered for specific subsystems.

## Supported editor concepts

| Editor | Typical use |
| --- | --- |
| Main admin menu | Navigate plugin tools and player controls |
| Quest editor | Create quests, rewards, command actions and lines |
| NPC shop editor | Choose functions, edit categories, copy custom items |
| EXP-crystal editor | Tune enabled skills, chances and ranges |
| Boss spawner tools | Create or manage encounter locations |
| World shrine tools | Test placement and monitor structures |
| Player utilities | Award levels, mana, souls or special items |

## Editing items

When an interface copies an item from an administrator's inventory, it should store the complete `ItemStack`, including its persistent metadata. This is particularly important for LevelCraft gear, custom enchantments and third-party items.

## Editing commands

A GUI can prompt for console commands through chat input. Test reward commands with a harmless command first and check placeholder replacement before adding high-impact operations.

## Safe testing steps

1. Duplicate a test definition rather than changing a production NPC or quest.
2. Make a small edit and reload only that feature.
3. Check UI display, reward delivery and saved YAML.
4. Restart once to ensure persistence.
5. Remove test data after confirming that the editor performed correctly.

If a GUI fails to open, verify that the relevant manager initialised and is registered as an event listener. Also check the appropriate permission node.

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
