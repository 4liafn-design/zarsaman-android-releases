# Release procedure

1. Identify the exact approved APK, version, package ID, signing certificate and full SHA-256. Do not rebuild an approved artifact merely to publish it.
2. Verify all applicable acceptance gates. Record PASS, NOT TESTED and BLOCKED honestly. Provider acceptance, physical notification receipt, normal in-app navigation and an actual notification tap are distinct checks. A simulation must not be presented as a physical tap.
3. Obtain any required explicit Owner decision for an unmet acceptance condition. Do not silently waive a gate.
4. Check both existing tags and releases. Never overwrite an existing tag, release or asset without separate authorization.
5. Publish only the approved APK and its SHA-256 checksum, with accurate version, signing/environment notes, installation instructions and known limitations. Mark test releases as pre-releases.
6. Download the public release asset without authentication and verify its complete SHA-256 against the approved artifact. Confirm the release and download URLs work before sharing them.
7. Generate a WhatsApp sharing link only from the verified public download/release URL.

## Installation

Download the APK and checksum from the same release. Verify the checksum before installing. Android may require permission to install applications from the selected browser or file manager; this is the user's choice. Never disable device-wide security protections. Retain a backup of important app data before an upgrade.

## Repository boundaries

Allowed: public release documentation, approved APKs, checksum files and public release notes.

Forbidden: application/backend source, signing keys, service-account files, passwords, tokens, production configuration, private reports, account information or device identifiers.

Repository creation and metadata preparation alone do not authorize uploading or publishing an APK.
