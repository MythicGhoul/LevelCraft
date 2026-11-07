# Parties & shared XP

Parties provide a lightweight way to group for exploration or combat and reward cooperation.

## How sharing works

A referenced design grants the player who earned an XP award its full value, while nearby qualifying party members can receive a **50% shared amount**. Because multipliers and event routing can interact, parties should be tested using the installed build rather than assuming that all XP actions are shared.

## Core concepts

- A party leader manages invitations and membership.
- Party chat provides a private group channel.
- Proximity determines which allies are eligible for nearby XP.
- Party data and rank or clan membership are separate.

## Commands

The referenced manifest registers `/party` and the alias `/p`. Exact subcommands depend on the party command implementation, but usually cover invitations, joining/leaving and chat. See in-game `/party` help.

## Permissions

`lc.party.use` and `lc.party.chat` are player-default permissions in the referenced manifest; `lc.party.admin` defaults to operator.

See [XP levels](../progression/leveling.md).

---

[← Documentation contents](../README.md) · [Project homepage](../../README.md)
