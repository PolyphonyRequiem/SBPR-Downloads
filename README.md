# Niflheim-Prelude

[Download the current Windows or Linux launcher](https://github.com/PolyphonyRequiem/SBPR-Downloads/releases/tag/launcher-0.1.6).

**Production:** `Niflheim-Prelude`, `50.52.127.244:2476`. This is the existing world,
not the separate playtest. No world reset, character reset or save rollback.

**Current release:** launcher **0.1.6**, client/server mod **0.2.51**, server-only
Eternal Flame **1.0.1**. Valheim **1.0.12 / network40**, Steam build `25253764`.
Trailborne is active; Homestead Stones remain disabled.

## Update and join

1. Sign into Steam and finish Valheim updates, then leave Valheim closed.
2. **Launcher 0.1.5 or earlier needs one manual bootstrap:** close the old launcher,
   download the complete Windows `SBPR.Launcher-0.1.6-win-x64.zip` or Linux
   `SBPR.Launcher-0.1.6-linux-x64.tar.gz` archive and extract it. Older launchers
   cannot self-update to 0.1.6. The `*-update.zip` assets are for launcher-managed
   updates, not manual installation.
3. Open launcher 0.1.6 and confirm **Prelude**, not **Prelude Playtest**. If using
   an existing managed game, select that SAME folder in Settings; do not install
   into Steam or a separate playtest folder.
4. New players: review the default `SBPR/prelude/game` destination, grant consent
   and Install. No manual mod ZIP is required.
5. Use **Play** or **Update & play**, choose your character in Valheim and enter
   the unchanged server password supplied privately by Daniel.

Always use the launcher before joining so your modpack matches production.
Install/update does not move or reset Steam files, characters or world saves.
Separate game folders do not isolate Steam Cloud. The invited playtest remains a
separate launcher/receipt/destination on port2486; it is not production.

## Launcher updates

Launcher 0.1.6 has separate launcher and modpack **Check** buttons. Checking reads
live release information; it does not install an update or start the game.
After the one-time manual bootstrap, future approved launcher updates use the
separate signed `prelude-launcher-release.json` feed. Choose **Update launcher &
restart** explicitly to apply an available launcher update. Modpack updates still
use **Update & play** and the unchanged `prelude-release.json` feed.

Launcher updates replace the launcher at the same path while preserving local
configuration and unowned files. If an update fails, retain Details and recovery
folders; do not delete them or your saves as a workaround.

## Changes

Launcher 0.1.6 adds authenticated self-update, independent live version checks and
recovery for failed replacement startup. This is a launcher-only release; the
following modpack 0.2.51 changes remain unchanged:

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
Windows Security. Manual Linux archives are unsigned; future launcher-managed
updates on both platforms are authenticated by the signed launcher feed and its
package hashes. SHA-256 sidecars accompany all four release archives. Dependency
licences and PLAYER-START.txt are included.

## Verification and support

Launcher 0.1.6 passed native Linux same-path update, refused-start rollback and
interrupted-update recovery checks. Published archives were anonymously downloaded
and hash-verified; Windows publisher signatures and timestamps were verified.
**Native Windows launcher execution has not been exercised.**

For modpack 0.2.51, native bundle coexistence/menu checks and real Linux launcher
install/update/game launch passed. Windows portal travel/logout replay remains
unverified; the owner explicitly authorized production promotion. If a portal
hangs, stop retrying and retain full BepInEx/LogOutput.log and Player.log. For
installer failures, share Details and preserve recovery folders; do not delete
caches or saves as a workaround.

The activation handshake is a mod-presence/compatibility gate, not cryptographic
attestation or exact package-version enforcement. Use the launcher for every join.
Only permitted release artifacts and feed metadata are published here; no private
source history, game binaries, saves or passwords are redistributed.

Operator note: modpack approval expires at `expiresUtc` in `prelude-release.json`;
launcher approval has its own `expiresUtc` inside the signed payload of
`prelude-launcher-release.json`. Renew each before its timestamp. No automatic
renewal is configured.
