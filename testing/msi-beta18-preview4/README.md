# FluJado beta.18 — MSI Preview 4

Separate Windows 64-bit installer preview, 19 October 2026. The regular beta download and automatic update feed are unchanged.

## Changes since Preview 3

- Uninstall now uses the same FluJado visual style as the installer, with progress and a clear completion screen and Finish button.
- Start menu maintenance shortcuts use a consoleless starter to launch the maintenance window without a PowerShell console flash.
- **Remove all Hub data and the local licence** now also removes the local licence storage for this Windows account. **Keep my data and licence** remains the default.

## Test on your other PC

1. Close FluJado. Download and run **FluJado-beta.18-MSI-Preview-4.msi**. If setting up a new PC, install your simulator software and connectors first.
2. Choose the installation location and shortcuts. Keep `GolfSimHub` as the final folder name.
3. Open FluJado and check that existing settings, flows and licence remain available after installation.
4. Close FluJado and open **Start menu > FluJado > Uninstall FluJado (data options)**. Check the appearance and whether a console window appears.
5. On a disposable test installation, test uninstall with the desired data option. Confirm that a clear **Uninstall complete** screen appears and Finish closes it.

**Deleting all data is permanent.** It removes settings, saved flows, artwork and local licence data, including the licence shared by other Hub installations on the same Windows account. It does not release the online activation. Deactivate in the Hub first if you want to move an activation to another PC. Simulator software is left untouched.

Removing through Windows Apps or the native MSI maintenance dialog keeps data by default. Use the Start menu shortcut for the full data-choice window.

Please report the installation location, whether the maintenance window opened without a console, whether completion was clear, and whether your selected data option worked. Do not send passwords or licence keys. If blocked by antivirus, stop and report the exact message; do not disable protection.

## Validation

Isolated tests passed for installation, shortcuts, keep/delete using fictitious licence files, repair, upgrade, cancellation, recovery after three injected transaction failures, and path/junction safeguards. Consoleless launch was tested with harmless fixture scripts. Maintenance handlers and rendered screens were checked with controlled test actions. A second-PC visual test is still requested; power loss was not simulated.

This is an unsigned installer preview, not a new regular beta release. The installer checksum is in `SHA256SUMS.txt`.
