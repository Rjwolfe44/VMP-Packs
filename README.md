# VMP-Packs

Pack definitions, signed locks and server lists for the [VMP Launcher](https://github.com/Rjwolfe44/VMPLauncher).

- `catalog.json` lists the packs. The launcher reads it from this repository's raw URL.
- `packs/<id>/channel.json` points at the current immutable lock (by version and SHA-256).
- `packs/<id>/<version>/` holds that version's lock, inventory, server policy and settings template. Only the current version is kept in this repository.
- `packs/<id>/servers.json` is the live server directory (routes, required build), re-signed on every change.
- `packs/<id>/KSPModControl.xml` is the server policy of the current version, and `packs/<id>/CHANGELOG.md` lists what changed between versions.
- `packs/<id>/<id>.vmpack.json` is the pack definition the current version was built from, and `packs/<id>/share/<id>.vmpack` is the small file players can import to find the pack.
- `library/library.json` is the signed list of the maintainer's own KSP mods that the launcher shows on its Mods page.

Everything that the launcher trusts is signed with the publisher key `vmp-host-2026a` (ECDSA P-256); the launcher ships the public key.
Files are served byte for byte from `raw.githubusercontent.com` and some are signed over their exact bytes, so `.gitattributes` disables line-ending conversion.
No passwords live here. Private packages are never uploaded.

The repository is written by `vmpl publish` of the launcher; see its README for the release flow. Do not edit the signed files by hand.
