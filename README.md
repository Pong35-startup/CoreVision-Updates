# CoreVision-Updates

## Stable Windows releases

The repository's GitHub remote is `Pong35-startup/CoreVision-Updates`. Stable version tags in the form `vMAJOR.MINOR.PATCH` create a **draft** GitHub Release. Prerelease tags such as `v1.0.0-beta` are rejected. Draft releases are not available to users until you upload the installer and publish the release.

To prepare the first release:

1. Merge the stable-release workflow into `main`.
2. Create and push the first stable tag from the commit you want to release:

   ```powershell
   git tag -a v1.0.0 -m "Release v1.0.0"
   git push origin v1.0.0
   ```

3. Wait for the **Stable release** workflow to create the draft, then open it under the repository's **Releases** page.
4. Upload `CoreVision-Setup.exe` to the draft and verify the file and release notes.
5. Publish the release when you approve it.

This repository currently contains no application source, installer, or auto-updater configuration. The workflow prepares the GitHub Release only; the installer must be built separately and uploaded manually. The `owner` value `YOUR_GITHUB_USERNAME` in the supplied example is a placeholder; for this repository, use `Pong35-startup`.
