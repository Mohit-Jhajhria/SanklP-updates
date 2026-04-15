# SanklP Updates

Auto-update release repository for the **SanklP** app — Moita Lab's collaborative exam preparation app for UPSC & RSSB aspirants.

## How It Works

The SanklP app checks this repository for new releases on every app open. If the release tag doesn't match the app's current version, it prompts the user to update.

## Creating a Release

1. Build the APK and/or EXE
2. Go to **Releases → Create a new release**
3. Set the **tag** to the new version (e.g. `v1.1`)
4. Write release notes describing what's new
5. Attach the APK (for Android) and/or EXE (for Windows) as assets
6. Publish the release

## Release Format

| Field | Example |
|---|---|
| Tag | `v1.1` |
| Title | `v1.1 — Bug Fixes & Improvements` |
| Assets | `sanklp.apk`, `sanklp.exe` |

> **Important:** The release tag must **not** match the app's `currentVersion` in `constants.dart` for the update to be detected. Update `currentVersion` in the app code to match the new tag before building.
