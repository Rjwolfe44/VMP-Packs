# VMP Train Career

## 2026.10.29.1 (2026-10-29)

Maintenance release: updates pack metadata. No mod or client changes.

- No module changes.
- Server policy: unchanged.

## 2026.10.28.2 (2026-10-28)

VMP client .10: automatic diagnostics. The game now writes a Health line to KSP.log every minute and, if it freezes, floods errors or the previous session crashed, sends a report (with ApexGuidance logs) to the host automatically; turn it off under Options. Also fixes Send logs to host, which could never start an upload.

- Updated: VMPCustom-VladMultiplayer 0.2.0-train.20261023.9 -> 0.2.0-train.20261023.10
- Server policy: 1 hash(es) updated, 0 DLL(s) added, 0 removed (223 mandatory).

## 2026.10.28.1 (2026-10-28)

VMP client .9: far less freezing in the VAB (no remote vessels loaded or re-downloaded in the builder, no repeated game saves after vessel loads, unchanged vessels are no longer reloaded) and the client now writes Slow operation and Frame stall lines to KSP.log.

- Updated: VMPCustom-VladMultiplayer 0.2.0-train.20261023.8 -> 0.2.0-train.20261023.9
- Server policy: 1 hash(es) updated, 0 DLL(s) added, 0 removed (223 mandatory).

## 2026.10.26.1 (2026-10-26)

Apex 2.15.0.286: faster ascents (up to 4x physics warp while climbing, shorter staging pause), landings that warp and actually land, many Apex ascent and Mission Director fixes. VMP client .8: your own dropped boosters and stages are no longer immortal, so they fall and tumble normally.

- Updated: VMPCustom-ApexGuidance 2.15.0.285+g272fcd7d -> 2.15.0.286+g98cbffea
- Updated: VMPCustom-VladMultiplayer 0.2.0-train.20261023.7 -> 0.2.0-train.20261023.8
- Private package(s) changed: ask the host for ApexGuidance-2.15.0.286_g98cbffea.zip.
- Server policy: 5 hash(es) updated, 0 DLL(s) added, 0 removed (223 mandatory).

## 2026.10.25.2 (2026-10-25)

Fixes the ZstdSharp load warning on the KSP loading screen (client 0.2.0-train.20261023.7 ships its missing System.Threading.Tasks.Extensions); snapshot compression is confirmed working in KSP.

- Updated: VMPCustom-VladMultiplayer 0.2.0-train.20261023.6 -> 0.2.0-train.20261023.7
- Server policy: 0 hash(es) updated, 223 DLL(s) added, 0 removed (223 mandatory).

## 2026.10.25.1 (2026-10-25)

Apex Orbit Matcher, contract orbits as targets, Pe/Ap change fixes; snapshot compression to cut bandwidth plus in-game send logs; Parallax: only large rocks are solid; new mods: SCANsat, Konstruction, Universal Storage II, CommNet Antennas Extension, Nexus.

- Added: CommNetAntennasExtension 2.1.9
- Added: Konstruction v112.0.1
- Added: SCANsat v21.1
- Added: SuperHeavyBoostersHistoricalNexus 2.0.200524
- Added: UniversalStorage2 4.0.4
- Added: USITools v112.0.1
- Updated: VMPCustom-ApexGuidance 2.15.0.284+g27d79cbd -> 2.15.0.285+g272fcd7d
- Updated: VMPCustom-VladMultiplayer 0.2.0-train.20261023.5 -> 0.2.0-train.20261023.6
- Overrides: +1 ~0 -0
- Private package(s) changed: ask the host for ApexGuidance-2.15.0.285_g272fcd7d.zip.
- Server policy: 0 hash(es) updated, 222 DLL(s) added, 0 removed (222 mandatory).

## 2026.10.24.4 (2026-10-24)

ApexGuidance 2.15.0.284: trips to Minmus cost much less fuel (about 945 m/s instead of up to about 1,190), a safe arrival a little off the planned height no longer stops the burn sequence, the landing autopilot warns you before a landing when you do not have enough fuel, and time warp no longer stops for minutes while the landing autopilot waits for its deorbit burn.

- Updated: VMPCustom-ApexGuidance 2.15.0.283+gc85ca58e -> 2.15.0.284+g27d79cbd
- Private package(s) changed: ask the host for ApexGuidance-2.15.0.284_g27d79cbd.zip.
- Server policy: 4 hash(es) updated, 0 DLL(s) added, 0 removed (212 mandatory).

## 2026.10.24.3 (2026-10-24)

Milestone and record rewards are no longer paid again every session: achievements are now saved and restored properly, and speed, altitude and distance records are kept up to date. The first session after this update earns them once more, then they stay.

- Updated: VMPCustom-VladMultiplayer 0.2.0-train.20261023.4 -> 0.2.0-train.20261023.5
- Server policy: 1 hash(es) updated, 0 DLL(s) added, 0 removed (212 mandatory).

## 2026.10.24.2 (2026-10-24)

Time warp no longer destroys your ship. Moon trips from ApexGuidance add a correction burn when needed and no longer fire the capture burn in empty space. Many autopilot fixes (ApexGuidance 2.15.0.283). VMP now has a Send logs to host button in Options, and a guard against jumping straight to top time warp.

- Updated: VMPCustom-ApexGuidance 2.15.0.282+gf690b00a -> 2.15.0.283+gc85ca58e
- Updated: VMPCustom-VladMultiplayer 0.2.0-train.20261023.3 -> 0.2.0-train.20261023.4
- Private package(s) changed: ask the host for ApexGuidance-2.15.0.283_gc85ca58e.zip.
- Server policy: 5 hash(es) updated, 0 DLL(s) added, 0 removed (212 mandatory).

## 2026.10.24.1 (2026-10-24)

ApexGuidance 2.15.0.282: fixes two repeating errors (the flight logging every tick, and the Mission Director in the VAB and SPH) and holds time warp at 1x during staging.

- Updated: VMPCustom-ApexGuidance 2.15.0.280+g91cbb1ba -> 2.15.0.282+gf690b00a
- Private package(s) changed: ask the host for ApexGuidance-2.15.0.282_gf690b00a.zip.
- Server policy: 4 hash(es) updated, 0 DLL(s) added, 0 removed (212 mandatory).

## 2026.10.23.5 (2026-10-23)

Fixes a crash that could disconnect a player while time warping. ApexGuidance 2.15.0.280: fixes the altitude rails-warp block below 100 km, restores HIGH warp mode in vacuum, and releases warp control when idle.

- Updated: VMPCustom-ApexGuidance 2.15.0.279+g30d4f9a6 -> 2.15.0.280+g91cbb1ba
- Updated: VMPCustom-VladMultiplayer 0.2.0-train.20261023.2 -> 0.2.0-train.20261023.3
- Private package(s) changed: ask the host for ApexGuidance-2.15.0.280_g91cbb1ba.zip.
- Server policy: 5 hash(es) updated, 0 DLL(s) added, 0 removed (212 mandatory).

## 2026.10.23.4 (2026-10-23)

New VMP toolbar button and flag art, and ApexGuidance updated to 2.15.0.279.

- Updated: VMPCustom-ApexGuidance 2.15.0.277+g9b362c4e -> 2.15.0.279+g30d4f9a6
- Updated: VMPCustom-VladMultiplayer 0.2.0-train.20261023.1 -> 0.2.0-train.20261023.2
- Private package(s) changed: ask the host for ApexGuidance-2.15.0.279_g30d4f9a6.zip.
- Server policy: 5 hash(es) updated, 0 DLL(s) added, 0 removed (212 mandatory).

## 2026.10.23.3 (2026-10-23)

Fix: an update no longer fails when KSP has redrawn a part icon (files in @thumbs folders, e.g. Mk3Expansion). No mod changes.

- No module changes.
- Server policy: unchanged.

## 2026.10.23.2 (2026-10-23)

VMP client 0.2.0-train.20261023.1: other players vessels show up again (fixed a vessel-sync crash), and career sync (launch pad and building upgrades, science) recovers by itself if it stalls. The server runs the matching build.

- Updated: VMPCustom-VladMultiplayer 0.2.0-train.20261022.1 -> 0.2.0-train.20261023.1
- Server policy: 1 hash(es) updated, 0 DLL(s) added, 0 removed (212 mandatory).

## 2026.10.23.1 (2026-10-23)

- Updated: VMPCustom-ApexGuidance 2.15.0.276+g5f225d83 -> 2.15.0.277+g9b362c4e
- Private package(s) changed: ask the host for ApexGuidance-2.15.0.277_g9b362c4e.zip.
- Server policy: 4 hash(es) updated, 0 DLL(s) added, 0 removed (212 mandatory).

## 2026.10.22.3 (2026-10-22)

ApexGuidance now downloads and updates automatically for friends who used an invite code (needs launcher 0.2.0). No mod changes.

- No module changes.
- Server policy: unchanged.

## 2026.10.22.2

ApexGuidance 2.15.0.276+g5f225d83 (rebuilt; private package, ask the host for the new zip). Server policy updated
for the three rebuilt ApexGuidance DLLs. Everything else unchanged; the update downloads nothing new from CKAN.

## 2026.10.22.1

First launcher-installable version: 180 CKAN mods pinned to exact versions, VMP client 0.2.0-train.20261022.1
(auto-join), ApexGuidance (private package handed out by the host), MechJebRPM disabled.
