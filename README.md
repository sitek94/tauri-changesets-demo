# Tauri Changesets Demo

Based on [minimal Tauri v2 demo](https://github.com/sitek94/tauri-minimal-demo) a simple demo with
releases managed by [changesets](https://github.com/changesets/changesets)

- On each push to main branch scans for changesets and creates a release if there are any
- Creates a Release PR with the new version
- After merging the release PR, the release is published to GitHub Releases with new app binaries
- App automatically checks for updates from GitHub Releases

## Setup

In order for this setup to work, you need to have a few things set up:

1. Rename every occurrence of `tauri-changesets-demo` to your app name
2. Generate a signing key for your app, e.g. using tauri signer

   ```bash
   bunx tauri signer generate -w ~/.tauri/tauri-demo.key
   ```

3. Update `plugins.updater.pubkey` in `tauri.conf.json` with the public key
4. Create

## Bootstrapped with Tauri v2

- [Tauri 2.0](https://tauri.app/)
