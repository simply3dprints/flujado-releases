# FluJado beta.18 — MSI Preview 6

Separate Windows 64-bit installer preview, 19 October 2026. The regular beta download and automatic update feed are unchanged.

## Changes since Preview 4

- Faster MSI ownership detection for opening FluJado, Uninstall and Repair. Only the FluJado product family is queried; Windows Installer still verifies the exact registered installation path.
- Uninstall and Repair windows now explicitly load the FluJado window icon.
- The final installation page offers **Start FluJado**, checked by default. Uncheck it to close the installer without opening the Hub. Quiet/passive updates, repair, removal and cancelled/failed installations do not start the Hub.
- Retains the Preview 4 uninstall design, clear completion page and explicit choice to keep data/licence or delete all local Hub data/licence.

## Test on the other PC

1. Close FluJado. Download and open **FluJado-beta.18-MSI-Preview-6.msi**. For a fresh setup, install your simulator software and connectors first.
2. Choose the installation location and shortcuts. Keep `GolfSimHub` as the final folder name.
3. Leave **Start FluJado** checked and select Finish. Check whether the Hub opens and note approximately how long it takes. Verify that existing settings, flows and licence are still available after installation.
4. Close the Hub, then open **Start menu > FluJado > Repair FluJado** and **Uninstall FluJado (data options)**. Check the window icons and how quickly the windows appear. Opening these windows alone does not repair or uninstall anything; Cancel closes them.
5. If testing uninstall on a disposable installation, check that the selected data option works and **Uninstall complete** appears with a Finish button.

**Deleting all data is permanent.** It also deletes local licence storage shared by Hub installations on the same Windows account. This does not release the online activation; deactivate in the Hub first if moving an activation to another PC. The default option keeps data and licence. Simulator software is left untouched.

Removing through Windows Apps or the native MSI maintenance dialog keeps data by default. Use the Start menu uninstall shortcut for the full data-choice screen.

Please report approximate opening times for the Hub, Repair and Uninstall, whether the icons appear, and whether Start FluJado works. Do not send passwords or licence keys. If antivirus blocks the installer, stop and report the exact message; do not disable protection.

## Validation

Isolated installation, repair, removal, upgrade, cancellation, injected transaction failure recovery, licence-data safeguards, window-icon and launch-checkbox checks passed. All 118 runtime files match the tested candidate. The identity lookup improved from about 207 ms to a median 6.5 ms on the development PC. One isolated validation-process comparison took about 4 seconds before and 2 seconds after; caching can affect these results. These are not guaranteed full application startup times on another PC. No actual Finish-click app launch or power-loss test was performed.

Unsigned installer preview, not a new regular beta release. See `SHA256SUMS.txt` for the checksum.
