# Tauri Changesets Demo

Based on [minimal Tauri v2 demo](https://github.com/sitek94/tauri-minimal-demo) a simple demo with
releases managed by [changesets](https://github.com/changesets/changesets)

- On each push to main branch scans for changesets and creates a release if there are any
- Creates a Release PR with the new version
- After merging the release PR, the release is published to GitHub Releases with new app binaries
- App automatically checks for updates from GitHub Releases

## Bootstrapped with Tauri v2

- [Tauri 2.0](https://tauri.app/)
