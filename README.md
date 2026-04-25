# OpenCode Mobile IPA

Auto-built iOS IPA for [Shahfarzane/opencode-mobile](https://github.com/Shahfarzane/opencode-mobile).

## Install via SideStore / AltStore

1. Open **SideStore** or **AltStore** on your iPhone
2. Go to **Sources** → **+** and paste:
   ```
   https://raw.githubusercontent.com/ssalonen/opencode-mobile-ipa/main/altstore-source.json
   ```
3. Find **OpenCode Mobile** in the Browse tab and tap **Install**

## Build from source

This repo contains a GitHub Actions workflow that:
1. Checks upstream (Shahfarzane/opencode-mobile) for new releases weekly
2. Builds an unsigned IPA using ad-hoc signing
3. Creates a GitHub release with the IPA
4. Updates `altstore-source.json` for SideStore/AltStore

See `.github/workflows/build.yml` for the build process.