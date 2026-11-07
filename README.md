# LevelCraft — Documentation

**Forge Your Path. Master Your Craft. Become Legend.**

A full multi-page, searchable documentation website for **LevelCraft**, an RPG progression plugin for Minecraft by **MythicGhoul**.

[![GitHub Pages](https://img.shields.io/badge/docs-GitHub%20Pages-8b5cf6)](https://mythicghoul.github.io/LevelCraft/) [![Minecraft](https://img.shields.io/badge/Minecraft-RPG-22d3ee)](https://www.spigotmc.org/resources/110629/)

### Explore the documentation

| Getting started | Player progression | Equipment & magic | Worlds & servers |
| --- | --- | --- | --- |
| [Install](docs/getting-started/installation.md) | [Eleven skills](docs/progression/skills/index.md) | [Rarity](docs/equipment/rarity.md) | [Corruption](docs/world/corruption.md) |
| [First character](docs/getting-started/first-character.md) | [Races](docs/progression/races.md) | [Power Level](docs/equipment/power-level.md) | [World shrines](docs/world/shrines.md) |
| [FAQs](docs/getting-started/faq.md) | [Paths](docs/progression/paths.md) | [Sockets](docs/equipment/sockets.md) | [Clans](docs/social/clans.md) |
| [Commands](docs/reference/commands.md) | [Quests](docs/quests/overview.md) | [Sorcery](docs/magic/overview.md) | [Admin guide](docs/administration/overview.md) |

**[Open the full navigation](docs/index.md)** — the GitHub Pages site adds a sidebar, top navigation, search, light/dark toggle, on-page contents and mobile layout.

## Publish as a GitHub Pages website

These files are designed to be **added to your existing `MythicGhoul/LevelCraft` repository**. Keep the existing `LICENSE` file; this package does not replace it. It does not include the private Java plugin source.

1. Download and extract the documentation ZIP.
2. Copy its **contents** (`docs/`, `.github/`, `mkdocs.yml`, `requirements-docs.txt`, `README.md`, etc.) into the root of your existing repo.
3. Commit and push to the **`main`** branch.
4. In **GitHub → repository Settings → Pages**, set **Build and deployment → Source → GitHub Actions**.
5. Open the **Actions** tab and check the “Deploy LevelCraft docs” run. The expected address is <https://mythicghoul.github.io/LevelCraft/>.

The `deploy-docs.yml` workflow builds MkDocs Material with search and publishes the result automatically on future `main` updates.

### Local preview (optional)

```bash
python -m venv .venv
# Activate .venv using the command appropriate for your OS
pip install -r requirements-docs.txt
mkdocs serve
```

Open `http://127.0.0.1:8000/` to preview changes. For a production-equivalent check, run `mkdocs build --strict`.

## What is included?

Documentation covers installation, character creation, eleven skill pages, milestones, Total Level, guild ranks, quests and promotion exams, quest walls, rarity, Power Level, socket gems, forging, Sorcery, spells, mana, world corruption, shrines, bosses, encounters, global events, Dynmap, BlueMap, economy, NPC shops, special items, parties, clans, trade, nametags, configuration, command/permission references, PlaceholderAPI, backups, performance and troubleshooting.

## Important release note

The **public GitHub repository has only the licence at the time these files were prepared**. The documentation has been based on public feature descriptions and LevelCraft project-development materials. Exact balance, available commands and integration support may vary by build. Read [Sources & verification](docs/about/sources.md) before treating version-dependent details as a release guarantee.

LevelCraft is an independent Minecraft plugin by MythicGhoul and is not affiliated with Mojang or Microsoft.
