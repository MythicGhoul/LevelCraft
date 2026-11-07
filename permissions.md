# Permissions reference

The following permissions come from a referenced `plugin.yml` with plugin version `6.4.2`. A permission manager can override plugin defaults, and recent command additions may define permissions in code or elsewhere.

## Player and staff permissions

| Node | Default | Use |
| --- | --- | --- |
| `lc.stats` | true | Character stats/profile GUI |
| `lc.top` | true | Leaderboards |
| `lc.forge` | true | Forge UI |
| `lc.guide` | true | Plugin guide |
| `lc.sockets` | true | Socket gem removal/interface |
| `lc.prestige` | true | Prestige UI |
| `lc.quests` | true | Quest UI |
| `lc.rank` | true | Rank/path UI |
| `lc.info` | true | Public character/rank info |
| `lc.admin` | op | Main administration |
| `lc.admin.quests` | op | Quest editor and admin operations |
| `lc.admin.boss` | op | Boss administration |
| `lc.party.use` | true | Party functions |
| `lc.party.chat` | true | Party chat |
| `lc.party.admin` | op | Party administration |

## Clan permissions

| Node | Default |
| --- | --- |
| `lc.clan.use` | true |
| `lc.clan.create` | true |
| `lc.clan.invite` | true |
| `lc.clan.join` | true |
| `lc.clan.kick` | true |
| `lc.clan.leave` | true |
| `lc.clan.disband` | true |
| `lc.clan.claim` | true |
| `lc.clan.unclaim` | true |
| `lc.clan.info` | true |
| `lc.clan.list` | true |
| `lc.clan.home` | true |
| `lc.clan.sethome` | true |
| `lc.clan.promote` | true |
| `lc.clan.demote` | true |
| `lc.clan.chat` | true |
| `lc.clan.members` | true |
| `lc.clan.map` | true |
| `lc.clan.admin` | op |
| `lc.clans.admin.bypass` | op |

> **Administrative bypass**
>
> `lc.clans.admin.bypass` bypasses clan protection rules in the referenced permission description. Give it only to trusted staff, and record actions taken inside player claims.


## Practical permission configuration

A minimal survival player normally needs standard LevelCraft UI permissions plus `lc.party.use` and the relevant clan permissions. Admins may need `lc.admin` **and** feature-specific admin nodes, not just operator status in a nonstandard permission setup.

Avoid setting every `lc.*` node to true for the default group: that can grant access to destructive commands and protection bypasses.

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
