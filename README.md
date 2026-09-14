# Niflheim-Prelude

[Download the current Windows or Linux launcher](https://github.com/PolyphonyRequiem/SBPR-Downloads/releases/latest).

**Production:** `Niflheim-Prelude`, `50.52.127.244:2476`. This is the existing world,
not the separate playtest. No world reset, character reset or save rollback.

**Current release:** launcher **0.1.5**, client/server mod **0.2.51**, server-only
Eternal Flame **1.0.1**. Valheim **1.0.12 / network40**, Steam build `25253764`.
Trailborne is active; Homestead Stones remain disabled.

## Update and join

1. Sign into Steam and finish Valheim updates, then leave Valheim closed.
2. Existing players: open the production launcher and choose **Update & play**.
   Existing launcher0.1.4 can use this feed. Launcher0.1.5 adds complete trail-light
   bundle validation; its application update is a separate manual download.
3. Download/extract the complete new launcher archive if needed. Confirm **Prelude**,
   not **Prelude Playtest**. If using an existing managed game, select that SAME
   folder in Settings; do not install into Steam or a separate playtest folder.
4. New players: review the default `SBPR/prelude/game` destination, grant consent
   and Install. No manual mod ZIP is required.
5. Use **Play** or **Update & play**, choose your character in Valheim and enter
   the unchanged server password supplied privately by Daniel.

Always use the launcher before joining so your modpack matches production.
Install/update does not move or reset Steam files, characters or world saves.
Separate game folders do not isolate Steam Cloud. The invited playtest remains a
separate launcher/receipt/destination on port2486; it is not production.

## Changes

Three Spade trail lights and Leather Straps (1 Leather Scraps -> 5 at Explorer's
Bench). Three-Legged Torch Stand is the standard new light. Old Path Lamps no
longer appear for new building but retain their saved identity, appearance,
footprint and fuel behavior. Field Local Maps hold a random angle per opening;
Surveyor's Table heading behavior remains. The tent/vendor asset archive collision
implicated in portal loading is repaired. Server admission gates are retained.
Eternal Flame supports all Trailborne torches on the server.

## Windows security

Owned Windows launcher PE files are Authenticode-signed by **Daniel Green**, with
Microsoft timestamps. A valid new build can still receive SmartScreen reputation
prompts. Stop on an invalid signature or unexpected publisher; do not disable
Windows Security. Linux archives are unsigned. Dependency licences and
PLAYER-START.txt are included.

## Verification and support

Native bundle coexistence/menu checks and real Linux launcher install/update/game
launch passed. Windows portal travel/logout replay remains unverified; the owner
explicitly authorized production promotion. If a portal hangs, stop retrying and
retain full BepInEx/LogOutput.log and Player.log. For installer failures, share
Details and preserve recovery folders; do not delete caches or saves as a workaround.

The activation handshake is a mod-presence/compatibility gate, not cryptographic
attestation or exact package-version enforcement. Use the launcher for every join.
Only permitted release artifacts and feed metadata are published here; no private
source history, game binaries, saves or passwords are redistributed.

Operator note: approval expires at `expiresUtc` in `prelude-release.json`; renew
before that timestamp. No automatic renewal is configured.
