# Niflheim-Prelude

[Download the current Windows or Linux launcher](https://github.com/PolyphonyRequiem/SBPR-Downloads/releases/latest).

**Production server:** `Niflheim-Prelude`, `50.52.127.244:2476`.
This is the existing Prelude world, not `trailborne-test`. The server world and player saves have not been reset.

**Current release:** launcher **0.1.4**, Trailborne modpack **0.2.48**, Valheim **1.0.12 / network 40** (Steam client build `25253764`). Trailborne is enabled; Homestead Stones remain disabled. Existing server-side helpers are retained.

## Join

1. Update Valheim in Steam and sign into the account that owns it. Leave Valheim closed while installing/updating.
2. Download and extract the complete launcher archive for your OS. Run `SBPR.Launcher.exe` on Windows or `SBPR.Launcher` on Linux.
3. For a first installation, review the separate game folder and disk requirement, then give consent and install. Correct paths in Settings only if needed.
4. Existing launcher-managed installations update in the **same folder**. Do not choose a new game folder just because a release changed. If necessary, select the existing managed folder in Settings.
5. Choose **Play** or **Update & play**. Pick your character in Valheim, press Start, and enter the server password supplied privately by Daniel.

The launcher downloads the approved modpack automatically; players do not need to supply a ZIP. Steam files, characters, inventory and exploration saves are not moved or reset by installation. The production feed now targets Prelude on port 2476, not the former playtest on 2486.

## Windows security

The owned Windows launcher files are Authenticode-signed by **Daniel Green**, with Microsoft timestamps. A newly signed build can still show SmartScreen's reputation warning. Verify the source and publisher. An invalid signature or unexpected publisher is a reason to stop, not disable Windows Security.

Linux launcher archives are unsigned. The archives include dependency licences and PLAYER-START.txt.

## Updates and support

Managed game/modpack updates are automatic after initial consent. Updating the launcher application itself is currently manual: obtain the latest complete archive from the download link above. If an operation fails, open Details and share the error with Daniel; do not delete saves or installation folders.

The server startup and release/download integrity have been verified. A Windows launcher-mediated join remains a manual acceptance check; cross-building and signature checks are not Windows runtime verification.

Only release artifacts and feed metadata are published here. No game binaries, private source history, saves or passwords are redistributed.

Operator note: release approval is bounded by `expiresUtc` in `prelude-release.json`; renew or replace it before **2026-10-14**. No automatic approval renewal is configured.
