# Administrative security

RPG progression systems have many persistent items, rewards and permission-sensitive actions. Administrative access should be treated with the same care as world-editing or economy controls.

## Key safeguards

- Grant only the permissions needed for each staff role.
- Restrict destructive operations such as world core manipulation, boss spawning and direct player-level changes.
- Keep `lc.clans.admin.bypass` away from ordinary players.
- Store Discord webhooks and credentials only in server-side files, never in public documentation.
- Validate item reward serialization, especially when third-party custom items are accepted.
- Revalidate trade confirmation and offer consistency server-side.
- Record important admin actions and maintain backups for rollback.

## Public repository policy

This documentation package is designed for a **public** GitHub repo. Do not add the full plugin source, player data, shop coordinates, resource pack credentials or server config secrets unless that release is intentionally public and legally appropriate.

## Licence

Your existing repository declares EPL-2.0. This package does not replace that `LICENSE`; see [Licence and publication](../about/licence.md) before publishing code or compiled JARs under the same repository.
