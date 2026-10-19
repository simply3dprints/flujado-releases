# FluJado beta.18 — MSI Preview 7

Separate Windows 64-bit installer preview, 19 October 2026. The regular beta download and automatic update feed are unchanged.

## Fix since Preview 6

Corrects the final **Start FluJado** action. Previously the box could be checked while Finish closed the installer without opening the Hub. The native Windows Installer file reference is now passed correctly. All 118 application runtime files are unchanged from Preview 6, retaining the faster startup checks, window icons and improved uninstall window.

## Test on the other PC

1. Close FluJado. Download and open **FluJado-beta.18-MSI-Preview-7.msi**. For a fresh setup, install your simulator software and connectors first.
2. Choose your installation location and shortcuts. Keep `GolfSimHub` as the final folder name.
3. On the last page, leave **Start FluJado** checked and select **Finish**. Confirm that FluJado opens automatically and your existing settings, flows and licence are still available.
4. If testing another installation, uncheck **Start FluJado** before Finish and confirm that the installer closes without starting the Hub.

Please report whether checked Finish starts the Hub and approximately how long it takes. Do not send passwords or licence keys. If antivirus blocks the installer, stop and report the exact message; do not disable protection.

## Uninstall behaviour retained

Use **Start menu > FluJado > Uninstall FluJado (data options)** for the data-choice window. Keeping data and licence remains the default. **Deleting all data is permanent** and also removes local licence storage shared by Hub installations on the same Windows account. It does not release the online activation; deactivate in the Hub first if moving an activation to another PC. Simulator software is left untouched. Removing through Windows Apps or native MSI maintenance keeps data by default.

## Validation

The old failure was reproduced through the real Windows Installer Finish button using a harmless local test executable. With the corrected reference, checked Finish launched the test executable from a path containing spaces; unchecked Finish did not. This test used an isolated final-page package without executing an installation through the UI. The actual Hub launch on the other PC still needs confirmation.

Wizard navigation, seven launch conditions, actual silent installation, repair and data keep/delete tests with fictitious licences passed. The distributable contains the real unchanged application runtime, not the test executable. Repair, removal, quiet/passive updates and cancelled/failed installations do not launch the Hub.

Unsigned installer preview, not a new regular beta release. See `SHA256SUMS.txt` for the checksum.
