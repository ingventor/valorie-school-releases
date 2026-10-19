# MindAlign School for Windows

Formerly Valorie School. This repository contains only Windows installers, signed release metadata, the public verification key and release guidance. Application source, teacher settings, credentials and school information are private.

## Current pilot

[MindAlign 0.3.3](https://github.com/ingventor/valorie-school-releases/releases/tag/v0.3.3) introduces the MindAlign app name, MindAlign.exe client, matching artwork and owned-shortcut migration. Normal downloads use MindAlign-0.3.3-Setup.exe. ValorieSchool-0.3.3-Setup.exe is an IDENTICAL compatibility alias for existing updater URL validation, not another application.

Both files are 171809168 bytes, SHA-256 3ea0f598f80e89262bb2785acc85134dc39067ddcaf2d16c3b7b21cf82e64e41. Revision-5 candidate-legacy.json binds the old basename accepted through 0.3.2; candidate-mindalign.json binds the new basename. Root candidate.json uses the compatibility envelope. New clients accept only these exact versioned names in this repository. Do not trust a replacement key delivered alongside a binary; verify the previously pinned key through the master handoff.

0.3.0 and 0.3.1 remain HOLD for their microphone interruption. 0.3.2 introduced output-only muting. Native microphone, full teacher-session expiry, reboot/sleep, upgrade and rollback acceptance remain required. Use one school-approved Windows 11 x64 pilot. Preserve protected recovery/code/deadline state, do not uninstall first. Old service/state identifiers remain for compatibility. The EXE includes its runtime; no GitHub login or SDK is needed on clients.

## Update channel

Approved clients poll stable.json hourly or on Check for updates. Only signed, versioned, exact-size/hash installers are accepted. Active teacher sessions finish before installation. Offline or rejected updates leave installed protection in place. Teacher access never disables permanent filtering.

candidate.json is NOT an approved feed. stable.json is intentionally absent pending native evidence review. The channel has no per-PC rollout targeting. This candidate has NOT been automatically installed by publication, and manual installation does not prove the automatic updater.

The RSA update signature is NOT Windows Authenticode publisher signing or SmartScreen reputation. IT must verify the pinned key, signature, expiry and hash, run --check-package and approve the pilot. Stop on mismatches, missing recovery or protection/audio regressions. Do not bypass an unverified publisher prompt.
