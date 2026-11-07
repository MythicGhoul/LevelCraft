# Maintaining the LevelCraft documentation

1. Make small edits in the relevant `docs/**/*.md` page. Keep one feature per page.
2. Update the `nav:` list in `mkdocs.yml` when adding, moving or deleting a page.
3. Check release notes/source before asserting exact numbers, commands or permissions.
4. When documenting config fields, copy the **key spelling** from the current generated YAML and include only minimal, clearly-labelled excerpts.
5. Run `mkdocs build --strict`; fix broken navigation links or missing pages.
6. Update `docs/about/changelog.md` after significant documentation changes.
7. Never commit private player data, economy credentials, webhooks or the LevelCraft private source unless separately approved.

Suggested documentation headings: **What it does**, **How to use it**, **Requirements**, **Configuration**, **Common issues** and **Related systems**.
