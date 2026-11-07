# PlaceholderAPI reference

When PlaceholderAPI is installed, LevelCraft exposes values to scoreboards, nameplates, tab lists and chat formats. The referenced expansion uses the namespace **`levelcraft`**.

## Character identity

```text
%levelcraft_race%
%levelcraft_race_display%
%levelcraft_race_id%
%levelcraft_race_title%
%levelcraft_race_drawback%
%levelcraft_race_drawback_description%
%levelcraft_path%
%levelcraft_rank_path%
%levelcraft_path_display%
%levelcraft_path_primary_skill%
%levelcraft_path_secondary_skill%
%levelcraft_title%
%levelcraft_rank_title%
%levelcraft_guild_rank%
%levelcraft_guild_rank_display%
```

## Levels, skills and mastery

```text
%levelcraft_total_level%
%levelcraft_total_level_max%
%levelcraft_total_progress%
%levelcraft_total_progress_percent%
%levelcraft_combat_level%
%levelcraft_mining_level%
%levelcraft_woodcutting_level%
%levelcraft_farming_level%
%levelcraft_fishing_level%
%levelcraft_hunting_level%
%levelcraft_smithing_level%
%levelcraft_exploration_level%
%levelcraft_excavation_level%
%levelcraft_crafting_level%
%levelcraft_sorcery_level%
```

Dynamic skill placeholders use these supported suffixes:

```text
%levelcraft_skill_<skill>_level%
%levelcraft_skill_<skill>_xp%
%levelcraft_skill_<skill>_xp_required%
%levelcraft_skill_<skill>_xp_remaining%
%levelcraft_skill_<skill>_progress_percent%
```

Replace `<skill>` with a lower-case skill ID, for example `mining`. Angle brackets in this block are *template placeholders*, not characters to send to PlaceholderAPI.

## Health, mana and equipment

```text
%levelcraft_health%
%levelcraft_max_health%
%levelcraft_health_display%
%levelcraft_health_percent%
%levelcraft_mana%
%levelcraft_max_mana%
%levelcraft_mana_regen%
%levelcraft_mana_display%
%levelcraft_mana_percent%
%levelcraft_held_item_power%
%levelcraft_held_item_sockets%
%levelcraft_held_item_gems%
```

## Prestige, souls and progression

```text
%levelcraft_prestige%
%levelcraft_prestige_level%
%levelcraft_prestige_xp_boost_percent%
%levelcraft_souls%
%levelcraft_max_souls%
%levelcraft_ascension_title%
%levelcraft_ascension_points%
%levelcraft_prestige_score%
%levelcraft_prestige_score_required%
```

## Parties, quests and spells

```text
%levelcraft_in_party%
%levelcraft_party_id%
%levelcraft_party_size%
%levelcraft_party_online%
%levelcraft_party_leader%
%levelcraft_party_is_leader%
%levelcraft_quest_tier%
%levelcraft_quests_total%
%levelcraft_quests_active%
%levelcraft_quests_completed%
%levelcraft_quests_ready%
%levelcraft_spells_total%
%levelcraft_spells_known%
%levelcraft_spells_usable%
%levelcraft_wand_spell%
%levelcraft_spell_loadout_1%
```

Dynamic quest/spell patterns:

```text
%levelcraft_quest_<quest-id>_active%
%levelcraft_quest_<quest-id>_progress%
%levelcraft_quest_<quest-id>_required%
%levelcraft_quest_<quest-id>_completed%
%levelcraft_quest_<quest-id>_completed_times%
%levelcraft_spell_<spell-id>_known%
%levelcraft_spell_<spell-id>_usable%
```

The referenced expansion also provides clan, boss-spawner and leaderboard families with ID/index-specific suffixes.

## World and event state

```text
%levelcraft_xp_event_active%
%levelcraft_xp_event_multiplier%
%levelcraft_xp_event_remaining%
%levelcraft_blood_moon_active%
%levelcraft_blood_moon_remaining%
%levelcraft_fishing_event_active%
%levelcraft_fishing_event_remaining%
%levelcraft_fishing_event_player_catches%
%levelcraft_encounters_active%
%levelcraft_corruption_cores%
%levelcraft_corruption_here%
%levelcraft_shrines_total%
%levelcraft_shrines_active%
%levelcraft_onboarding_complete%
%levelcraft_npc_shops_count%
%levelcraft_transmutation_balance%
%levelcraft_money%
```

## Testing placeholders

Use a PlaceholderAPI test command such as `/papi parse me %levelcraft_total_level%` if supported by your PlaceholderAPI version. If it remains literal, check that PlaceholderAPI loaded, the LevelCraft expansion registered successfully and the identifier matches the source.
