# FluJado Golf Sim Hub — beta.18.1

[Download Windows installer (MSI)](downloads/FluJado-Golf-Sim-Hub-0.9.0-beta.18.1.msi) · [Getting started](docs/beta.18.1/GETTING-STARTED.txt) · [Checksums](docs/beta.18.1/SHA256SUMS.txt)

## New in beta.18.1

- MSI is now the standard installer, with the externally confirmed Preview 7 wizard, custom location, optional shortcuts and working **Start FluJado** checkbox on Finish.
- Faster startup checks, FluJado window icons and improved Repair/Uninstall windows with a clear completion screen.
- Updates retain settings, workflows, artwork and licence. The Start menu uninstaller defaults to keeping data; explicit delete-all also removes the local licence. Simulator software stays untouched.
- MSI update recovery and one-time EXE-to-MSI migration have isolated installation, cancellation, interruption and data-preservation tests.

## Existing beta users

**Beta.18 EXE:** use the update notice in the Hub. A one-time MSI transition starter creates a verified private backup and opens this exact MSI on the existing path. After migration, updates use MSI directly. This bootstrapper is only for the legacy updater; new installations should use the MSI download above.

**Already using an MSI preview:** install the new MSI or use the Hub's update notice. **Beta.17 or older:** the old updater may not parse dotted repair versions; create a private backup and install the MSI manually into the existing Hub folder. Do not uninstall first or delete data.

The Hub checks for a newer version about 15 seconds after opening and every six hours. Its update notice appears when no flow is active and Presentation mode is off. You choose when to install; simulator software is not stopped. The installers are currently unsigned.

## Earlier beta.18 fixes retained

- GSPro and other previously disabled built-in tiles are activated when selected in Guided setup. Choose your hardware profile and save; existing active workflows are preserved unless you explicitly select replacement.
- Missing required connector/program paths are reported on Golf setup, before screens and Movies & TV.
- Update checks support numeric beta repair revisions.

Install and activate simulator software and connectors first; verify a real shot outside the Hub. Vendor binaries and licences are not included. Keep private migration backups local and never send licence keys or passwords.

[Compatibility and test status](COMPATIBILITY.md) · [Release notes](docs/beta.18.1/RELEASE-NOTES.txt)

Existing VTrack Bridge automatic recognition remains experimental and untested with VTrack hardware. MSIX Toolkit support is not included in this release. [VTrack instructions (English)](docs/beta.17/VTRACK-BETA-TEST-EN.txt) · [Nederlands](docs/beta.17/VTRACK-BETA-TEST-NL.txt).

General illustrated guides (beta.15; use the release notes above for the wizard changes): [English](docs/beta.15/FluJado-Beta-User-Guide-EN.pdf) · [Nederlands](docs/beta.15/FluJado-Beta-Handleiding-NL.pdf) · [Connector guide](docs/beta.15/FluJado-Connector-Setup-Guide-EN.pdf).

Previous downloads remain available.
