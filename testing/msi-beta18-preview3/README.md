# FluJado beta.18 — MSI Preview 3

Separate installer preview for Windows 64-bit, 19 October 2026. The regular beta download and automatic update feed are unchanged.

## What to test

1. Install your simulator software and connectors first. Close FluJado before installing this preview.
2. Download **FluJado-beta.18-MSI-Preview-3.msi** and open it.
3. Follow the FluJado wizard. Try another installation location if desired; keep `GolfSimHub` as the final folder name.
4. Choose whether to add desktop and Start menu shortcuts. Check that Back/Next retain your choices.
5. Install, then open FluJado using your chosen shortcut. Confirm that your existing settings, flows and licence are still available when upgrading an existing installation.
6. The Start menu provides **Repair FluJado** and **Uninstall FluJado (data options)**. Uninstall defaults to keeping settings, saved flows and artwork. Deleting this installation's Hub data requires selecting the explicit delete option; licence data and simulator software are retained.

Removing through Windows Apps or the native MSI maintenance dialog keeps Hub data by default. Use the Start menu uninstall shortcut for the data-choice screen.

If the installation is blocked or fails, stop and share the exact message and installer version. Do not disable antivirus protection or send passwords or licence keys.

Please report: fresh install or upgrade, selected location, shortcuts created, whether settings/flows were retained, and any repair or uninstall issue. Choose data deletion only on a disposable test installation.

## Validation

Isolated tests passed for installation to a custom location, optional shortcuts, repair, data retention/deletion, major upgrade, cancellation and recovery from injected transaction failures. All 117 runtime files matched their expected hashes. These tests do not simulate a power loss. No simulator or connector was launched during these tests.

This is an unsigned MSI preview, not a new regular beta release. Check `SHA256SUMS.txt` for the installer checksum.
