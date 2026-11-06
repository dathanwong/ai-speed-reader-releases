# AI Speed Reader releases

This repository publishes macOS builds of AI Speed Reader. It does not contain source code. The app is private; these releases are the public update feed.

Installed copies check, with no token:

`https://api.github.com/repos/dathanwong/ai-speed-reader-releases/releases/latest`

Each release uses the same version tag as the private build (`v0.3.9`, and so on). The assets are:

- `AISpeedReader-macOS.zip` — the app the in-app updater downloads
- `AISpeedReader.dmg` — the drag-to-Applications disk image

The release notes include `SHA256` lines for those two files. The app checks the zip's code signature before it installs. It does not require a GitHub login.

## Install

1. Open the latest release and download `AISpeedReader.dmg`.
2. Open the disk image and drag **AI Speed Reader** to **Applications**.
3. Open it from Applications. On first launch, allow it in **System Settings > Privacy & Security** if macOS blocks the developer signature.
4. Grant **Accessibility** when asked. A re-signed update drops the previous grant, so enable AI Speed Reader again after installing.

The default shortcut is **Option + Space**. Hover a message, or highlight text, then press the shortcut.

## Updates

The app checks this feed while it is open, downloads quietly, and replaces itself when you quit or the next time it launches. **Restart to Update** is optional. Updates are never required.

If Check for Updates says it could not reach the update server, this repository has no published release yet, or the request was blocked. A 404 is not "you are already up to date."
