# FluJado beta.18 — MSI Preview 2

This is the newer, separately tested MSI package with managed MSI update recovery, repair and removal. It contains 116 application files. It is not the older MSI pilot and does not change the normal beta download or update feed.

## Test on another PC

1. Back up any existing Hub installation and its settings/licence privately. Finish the simulator session and close the Hub before installation.
2. The target is **%LOCALAPPDATA%\GolfSimHub**. If your existing Hub uses another folder, do not install over it with this preview.
3. If the previous MSI pilot is already installed, back up first, then remove that pilot through Windows Installed apps before installing Preview 2. It has the same numerical MSI version, so a direct same-version upgrade is blocked. Keep personal data.
4. Download [FluJado-beta.18-MSI-Preview-2.msi](./FluJado-beta.18-MSI-Preview-2.msi) and run it with Windows protection enabled. If protection blocks anything, stop and record the detection/affected file; do not add exclusions.
5. Open **%LOCALAPPDATA%\GolfSimHub\GolfSimHub.exe**. An existing shortcut for that folder also works. This preview does not create new shortcuts.
6. Check startup, settings/licence and your chosen simulator tiles. A first installation still requires your usual Hub setup and a valid licence/trial; no licences or tester data are included.
7. Report whether download, installation, startup and your settings work correctly, plus any exact error message. Never share licence keys or passwords.

## Maintenance status

The Hub version remains beta.18. MSI repair repairs the current version; it does not restore an older release. MSI removal keeps personal data and does not deactivate an online licence.

The normal update feed remains unchanged and does not yet offer MSI updates. The new updater will refuse an EXE update or an MSI update without a verified recovery MSI. Initial migration must save the verified MSI as its recovery source before future MSI updates are enabled; this preview is not an automatic fleet migration.

## Validation

Isolated tests passed for three interrupted transaction points, real cancellation (1602), retry, major upgrade/downgrade refusal, 116 runtime hashes, repair/removal, registration migration and separate updater processes at success and failure. Settings, licence fixtures and customized artwork were retained. Twelve actual WPF handler scenarios and rendered window images were reviewed. No physical power-loss test or live-desktop mouse walkthrough was performed.

Both MSI and application remain unsigned. The previous EXE is under Microsoft review; this package has not been approved by Microsoft. Local test results do not guarantee the same result on another PC.

SHA-256: `b58c5d33d693d3a3a35dc41468fd7cf78b73845b7c7ddd1bf0daf05b0a9e1fcc`
