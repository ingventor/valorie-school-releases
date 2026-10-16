# Valorie School for Windows

Public distribution only: signed release metadata, Windows installers and the
public verification key. Application source, teacher settings, credentials and
school information are not published here.

## Pilot build

The 0.3.0 prerelease is for one school-approved Windows 11 x64 pilot, not immediate
fleet rollout. It adds cinematic artwork and a full-application update button.
Existing 0.2.4/0.2.5 installations require a one-time administrator-approved
bootstrap. The EXE includes its runtime, no GitHub login or SDK is needed.

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
