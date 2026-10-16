# Valorie School for Windows

Public distribution only: signed release metadata, Windows installers and the
public verification key. Application source, teacher settings, credentials and
school information are not published here.

## Pilot build

0.3.0 and 0.3.1 are HOLD: their quiet mode also interrupted microphones.
Do not install them on additional PCs. The newer 0.3.2 prerelease corrects
output-only muting, retains the School open-book badge and preserves recovery
state. It needs one school-approved Windows 11 x64 pilot, not immediate fleet
rollout. Native microphone/output/expiry/recovery checks remain required.
Existing 0.2.4/0.2.5 installations require a one-time administrator-approved
bootstrap. The EXE includes its runtime, no GitHub login or SDK is needed.
The 0.3.0 pilot needs an in-place 0.3.2 candidate upgrade for native testing.
Do not uninstall first or remove its protected recovery backup.

The installer does not yet have Windows Authenticode publisher signing. IT must
verify the downloaded SHA-256 against the signed candidate manifest, check the
public key through the trusted master handoff, and approve the bootstrap.
Do not bypass an unverified publisher prompt.

## Update channel

Approved clients poll stable.json hourly or when Check for updates is pressed.
Only signed, versioned, exact-hash installers are accepted. Active teacher
sessions finish before installation. Unavailable or rejected updates retain
the installed protection. Teacher access never disables permanent filtering.

candidate.json is not an approved feed. stable.json is intentionally absent
until the master reviews native installation, reboot, expiry, upgrade and
rollback evidence. Publication/download is not proof of installation.

The update signature verifies the release channel. It is not an Authenticode
certificate or a claim of Windows SmartScreen reputation.
