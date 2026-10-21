# FluJado Golf Sim Hub — beta.18.5

[Download Windows installer (MSI)](downloads/FluJado-Golf-Sim-Hub-0.9.0-beta.18.5.msi) · [Getting started](docs/beta.18.5/GETTING-STARTED.txt) · [Checksums](docs/beta.18.5/SHA256SUMS.txt)

## New in beta.18.5

- Full removal now checks both known Windows licence stores. Invalid/linked paths are rejected; remaining or locked files cannot be reported as successfully removed. Keep-data remains the default; normal updates retain settings and licence.
- Isolated two-store removal, MSI first install/repair/upgrade and injected rollback tests passed.
- Post-reboot practice on 21 October passed: Muni ProTee VX, VX Muni/GSPro roundtrip, Muni Square Omni shots and Omni restart readiness. Fresh Hub installation on the existing PC passed; original settings and licence restored. No clean-Windows-PC or putting claim.
- [Current English instructions](docs/beta.18.5/GETTING-STARTED.txt) · [Nederlandse aanvulling](docs/beta.18.5/HANDLEIDING-AANVULLING-NL.txt) · [Connector update](docs/beta.18.5/CONNECTOR-GUIDE-UPDATE-EN.txt).

## Retained from beta.18.4

- Guarded Muni / ProTee VX recovery: if the rela plugin has not started Labs after 45 seconds of a matching stalled connection, start the configured Labs once. Existing, loading, updating or unreadable Labs processes are left alone.
- Three cold starts passed automatically in 58–61 seconds. The missing-Labs branch was tested with production-worker fixtures, including duplicate-start and transient-process guards; it was not needed or forced during these three starts.
- Settings, licence and custom workflows remain preserved. No new shot, putting, reboot or clean-PC hardware claim. Other simulator and Square routes are unchanged.

## Retained from beta.18.3

- Muni Golf Sim with ProTee VX and Square Omni via rela, with local port 9210, guarded startup and projector routing. Real shots passed for both.
- Muni to GSPro and back with ProTee VX passed with real shots. Square Omni switching with GSPro is excluded from this test scope.
- Fourteen other Muni profiles are **Not tested (assisted)**. These are inferred connector combinations; check the exact model and requirements in the compatibility table.
- Official Drills, Infinite Tees and Muni tile artwork; removed the PLAY label and corrupted arrow text.
- Updated Dutch/English guides, connector guide and test table. Settings, licence and custom workflows are retained.

One earlier VX startup was delayed before Labs appeared; beta.18.4 adds the guarded recovery described above. Subsequent automatic starts passed. The post-reboot Muni tests above now passed; putting and a clean-Windows-PC hardware test remain pending. No new Verified hardware claim.

## Existing beta users

**Beta.18 EXE:** use the update notice in the Hub. A one-time MSI transition starter creates a verified private backup and opens this exact MSI on the existing path. After migration, updates use MSI directly. This bootstrapper is only for the legacy updater; new installations should use the MSI download above.

**Already using an MSI preview:** install the new MSI or use the Hub's update notice. **Beta.17 or older:** the old updater may not parse dotted repair versions; create a private backup and install the MSI manually into the existing Hub folder. Do not uninstall first or delete data.

The Hub checks for a newer version about 15 seconds after opening and every six hours. Its update notice appears when no flow is active and Presentation mode is off. You choose when to install; simulator software is not stopped. The installers are currently unsigned.

## Earlier beta.18 fixes retained

- GSPro and other previously disabled built-in tiles are activated when selected in Guided setup. Choose your hardware profile and save; existing active workflows are preserved unless you explicitly select replacement.
- Missing required connector/program paths are reported on Golf setup, before screens and Movies & TV.
- Update checks support numeric beta repair revisions.

Install and activate simulator software and connectors first; verify a real shot outside the Hub. Vendor binaries and licences are not included. Keep private migration backups local and never send licence keys or passwords.

[Compatibility and test status](COMPATIBILITY.md) · [Release notes](docs/beta.18.5/RELEASE-NOTES.txt)

Existing VTrack Bridge automatic recognition remains experimental and untested with VTrack hardware. MSIX Toolkit support is not included in this release. [VTrack instructions (English)](docs/beta.18.3/VTRACK-BETA-TEST-EN.txt) · [Nederlands](docs/beta.18.3/VTRACK-BETA-TEST-NL.txt).

Illustrated beta.18.3 guides, updated for Drills, ShotForge, screens and MSI installation/recovery: [English](docs/beta.18.3/FluJado-Beta-User-Guide-EN.pdf) · [Nederlands](docs/beta.18.3/FluJado-Beta-Handleiding-NL.pdf) · [Connector guide](docs/beta.18.3/FluJado-Connector-Setup-Guide-EN.pdf).

Previous downloads remain available.
