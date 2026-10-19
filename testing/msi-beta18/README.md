# FluJado beta.18 — experimental MSI installer

This separate pilot uses the same 112 application files as beta.18, packaged with standard Windows Installer instead of the original self-extracting EXE. It does not change the normal beta download or automatic update feed.

## Before testing

- Back up your existing Hub installation, settings and licence privately.
- Check the existing installation folder. This MSI targets **%LOCALAPPDATA%\GolfSimHub** only. If your Hub is elsewhere, stop and report the location privately before installing.
- Wait until your simulator session has ended, then close the Hub and simulator apps before installing.
- Keep Windows security enabled. If downloading, installing or opening the Hub is blocked, stop and capture the detection name and affected file. Do not add exclusions or restore quarantined files.

## Install and check

1. Download [FluJado-0.9.0-beta.18-MSI-PILOT.msi](./FluJado-0.9.0-beta.18-MSI-PILOT.msi) and run it.
2. Open the Hub using your existing shortcut. The pilot does not create new shortcuts or launch the Hub automatically.
3. Confirm version **0.9.0-beta.18**, your settings and licence.
4. For the GSPro tile issue, use Guided setup, choose your actual launch monitor/connector route and GSPro, leave **Replace existing** off, and save. Check whether the GSPro tile appears and whether a missing connector is reported early.
5. Report download/install/start results, any security message and whether your settings and tile are correct. Never send passwords or licence keys.

## Validation and limitations

Isolated extraction verified all 112 runtime file hashes. Installation, upgrade over a beta.17 test copy, reinstallation and removal passed; five personal-data fixtures were preserved. The real installation, licence and simulator routes were not used.

A local Defender scan reported no threats on 19 October 2026 (engine 1.1.26090.9, definitions 1.461.100.0). This does not guarantee the same result on another PC. Both MSI and Hub are unsigned. The original EXE was submitted to Microsoft; review is pending. This MSI has not been cleared by Microsoft.

The package has no installer custom actions, services or drivers. It registers as a separate MSI product; migration of the legacy EXE updater/uninstaller is not included. It is a limited test, not a general rollout.

SHA-256: `f2f85fbcd557bdbc1465781b86ead10ff5a6d42f49886e66860fd843910145bd`
