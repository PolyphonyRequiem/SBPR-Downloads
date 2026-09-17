# Niflheim-Prelude

[Download the current Windows or Linux launcher](https://github.com/PolyphonyRequiem/SBPR-Downloads/releases/tag/launcher-0.1.6).

**Production:** `Niflheim-Prelude`, `50.52.127.244:2476`. This is the existing world,
not the separate playtest. No world reset, character reset or save rollback.

**Current release:** launcher **0.1.6**, client mod **0.2.56**, server mod **0.2.56**,
server-only Eternal Flame **1.0.1**. Valheim **1.0.14 / network40**, Steam build `25364265`.
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

## Prelude 0.2.56

- Local Map: right-click to read without equipping; M reopens a carried map. Comma/period rotate it. New approved framed-hide art and icon; add 6 Leather Straps to the map recipe. Existing map snapshots and saved identities remain.
- Explorer's Bench: approved compact table, icon and cylindrical collider. Existing station identity and recipe remain.
- Spade and Cartographer's Kit: approved new models and icons, with the equipped kit visible on the left hip. Add 3 Leather Straps to the Spade recipe and 6 to the Kit recipe.
- All four pigments: approved wooden-pot models and transparent inventory icons.
- Neck ink: new Ink Gland material and approved art. Ordinary Necks have a 50% base drop chance; normal starred/world resource scaling remains. One- and two-star Necks gain a weak two-shot ink attack with a brief slow and damage-over-time effect.
- Black Pigment now requires **1 Neck Ink Gland → 2 Black Pigment**, replacing Coal. Its description reads “A dark pigment, made from Neck ink.”

**Gameplay validation is deferred by Daniel's explicit instruction.** Build/package integrity and server startup are checked; this is not a completed gameplay/visual/multiplayer acceptance claim.

Fully close Valheim, let Steam finish its current Valheim update, then open the existing launcher, select **Prelude**, and use **Update & play**. Keep the same managed folder and character. Launcher 0.1.6 is unchanged. No world reset or save rollback.

### Previous release: 0.2.55

**0.2.55** combines longer-lived cairns with updated appearances for the three
existing trail lights and Leather Straps. No new recipes or pieces. Dry total
cairn lifetimes from full repair, including downgrades, are **2 / 5 / 9 / 15 / 28
real days** for tiers 1–5 at normal running-world clock speed. Sleep/time skips
still count; stopped servers do not age cairns. Rain wears lower tiers faster,
only while raining in player-loaded areas, with no unloaded rain backfill.

Fully close Valheim, then open the existing launcher, select **Prelude**, and use
**Update & play**. Keep the same managed folder and character. Launcher 0.1.6 is
unchanged. Gameplay and saved-instance validation follows this release; do not
read publication as a completed-playtesting claim.

### Previous release: 0.2.53

**0.2.53** corrects the Surveyor's Table from stone to wooden-furniture support.
Both client and server are updated; launcher 0.1.6 is unchanged. Fully exit
Valheim, then use **Prelude → Update & play** in the existing launcher. Keep
the same managed folder and character. No world reset or save migration.

The table keeps 800 HP, its recipe, saved identity and survey data format, and
still collapses when genuinely unsupported. Wood also lowers its outgoing
support capacity, so structures built atop tables may receive less support.

Source review, 1,992 tests, client/server builds, shipping-launcher package
validation and dedicated startup passed. Native placement/support, saved-table
and ownership-transfer tests remain unverified: the isolated test runtime failed
to start. The operator explicitly accepted that gap for release; this is not a
claim that every placement rejection or stone-edge case has been reproduced.

### Earlier updates

Client hotfix **0.2.52** fixes the Local Map and Surveyor's Table losing their
map raster after logout and rejoin in the same Valheim process. The viewer now
refreshes its copied material when the scene-owned shader changes. Fully exit
Valheim once to install the update using **Update & play**; no map recrafting,
save migration or server restart is needed. Launcher 0.1.6 is unchanged.

Launcher 0.1.6 provides authenticated self-update, independent live version checks
and recovery for failed replacement startup. Earlier modpack 0.2.51 content remains:

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

For client 0.2.52, the retained native regression fails the old DLL after relog
and passes both map modes through two bundle teardown/rejoin cycles on the new
DLL. The exact distributed package passes the shipping launcher 0.1.6 validator;
only the client plugin DLL and refreshed licence metadata change. This was an
isolated Linux Unity test, **not a Windows/D3D gameplay relog test**.

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
