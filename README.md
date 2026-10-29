# VMP-Packs

Pack definitions, signed locks and server lists for the [VMP Launcher](https://github.com/Rjwolfe44/VMPLauncher).

- `catalog.json` lists the packs. The launcher reads it from this repository's raw URL.
- `packs/<id>/channel.json` points at the current immutable lock (by version and SHA-256).
- `packs/<id>/<version>/` holds that version's lock, inventory, server policy and settings template.
- `packs/<id>/servers.json` is the live server directory (routes, required build), re-signed on every change.

Everything is signed with the publisher key `vmp-host-2026a` (ECDSA P-256); the launcher ships the public key.
No passwords live here. Private packages are never uploaded.
