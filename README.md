# FluJado Golf Sim Hub — beta.18.2

[Download Windows installer (MSI)](downloads/FluJado-Golf-Sim-Hub-0.9.0-beta.18.2.msi) · [Getting started](docs/beta.18.2/GETTING-STARTED.txt) · [Checksums](docs/beta.18.2/SHA256SUMS.txt)

## New in beta.18.2

- Drills support with ProTee VX and Square Omni via rela: real shots confirmed on both, with guarded startup, receiver checks and ProTee startup recovery.
- Fifteen additional Drills routes are available as **assisted, not hardware tested**. See the compatibility table for exact devices and limitations.
- Simulator windows inherit the selected projector screen. Drills leaves you in control of game selection; the Hub does not select Open Range.
- ShotForge connection/readiness improvements and early checks for conflicting rela plugins.
- MSI upgrade recovery corrected for added application files; isolated installation, repair, upgrade, cancellation and four rollback/retry interruption points passed.
- Updated Dutch/English user guides and connector guide. Settings, saved workflows and licence are retained on update. To adopt a changed preset, back up and explicitly select replacement in Guided setup.

ProTee VX switching Drills → GSPro → Drills was confirmed. Omni return to Drills was confirmed; a GSPro/Omni shot was not validated in that switching session. Additional profiles are not a hardware compatibility guarantee.

## Existing beta users

**Beta.18 EXE:** use the update notice in the Hub. A one-time MSI transition starter creates a verified private backup and opens this exact MSI on the existing path. After migration, updates use MSI directly. This bootstrapper is only for the legacy updater; new installations should use the MSI download above.

**Already using an MSI preview:** install the new MSI or use the Hub's update notice. **Beta.17 or older:** the old updater may not parse dotted repair versions; create a private backup and install the MSI manually into the existing Hub folder. Do not uninstall first or delete data.

The Hub checks for a newer version about 15 seconds after opening and every six hours. Its update notice appears when no flow is active and Presentation mode is off. You choose when to install; simulator software is not stopped. The installers are currently unsigned.

## Earlier beta.18 fixes retained

- GSPro and other previously disabled built-in tiles are activated when selected in Guided setup. Choose your hardware profile and save; existing active workflows are preserved unless you explicitly select replacement.
- Missing required connector/program paths are reported on Golf setup, before screens and Movies & TV.
- Update checks support numeric beta repair revisions.

Install and activate simulator software and connectors first; verify a real shot outside the Hub. Vendor binaries and licences are not included. Keep private migration backups local and never send licence keys or passwords.

[Compatibility and test status](COMPATIBILITY.md) · [Release notes](docs/beta.18.2/RELEASE-NOTES.txt)

Existing VTrack Bridge automatic recognition remains experimental and untested with VTrack hardware. MSIX Toolkit support is not included in this release. [VTrack instructions (English)](docs/beta.18.2/VTRACK-BETA-TEST-EN.txt) · [Nederlands](docs/beta.18.2/VTRACK-BETA-TEST-NL.txt).

Illustrated beta.18.2 guides, updated for Drills, ShotForge, screens and MSI installation/recovery: [English](docs/beta.18.2/FluJado-Beta-User-Guide-EN.pdf) · [Nederlands](docs/beta.18.2/FluJado-Beta-Handleiding-NL.pdf) · [Connector guide](docs/beta.18.2/FluJado-Connector-Setup-Guide-EN.pdf).

Previous downloads remain available.
