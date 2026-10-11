# tunnel-it desktop downloads

A free desktop dashboard for **Azure Dev Tunnels**, built with Tauri. Application source is maintained in a separate private repository. This repository distributes only public installers, checksums, and release notes.

**[Download the desktop app](https://github.com/awalakaushik/tunnel-it-releases/releases)** · **[Website and interactive demo](https://tunnel-it.netlify.app/)**

## Choose your installer

| Platform | Recommended asset | Alternative |
| --- | --- | --- |
| Windows 64-bit | tunnel-it-windows-x64.exe | .msi |
| macOS Apple Silicon (M1 and newer) | tunnel-it-macos-arm64.dmg | — |
| macOS Intel | tunnel-it-macos-x64.dmg | — |
| Linux 64-bit | tunnel-it-linux-x64.AppImage | .deb or .rpm |

Every release includes **SHA256SUMS.txt**. Releases are previews until code signing/notarization and installation/Azure smoke testing are complete. Current installers are unsigned; macOS builds are not notarized. OS security may block them. Do not disable security protections to install this preview.

## Set up Azure

1. Download and install the appropriate desktop build.
2. Install the official [Microsoft devtunnel CLI](https://learn.microsoft.com/en-us/azure/developer/dev-tunnels/get-started).
3. Open tunnel-it → Settings → Check installation → Sign in with Microsoft or GitHub.
4. Start your local server, create a profile with its ports, and choose Save & start.

Authenticated access is the default; public sharing requires an explicit choice. Quitting stops the app's tunnel host processes. tunnel-it adds no subscription or usage fee; Azure limits and terms apply. ngrok and Cloudflare Tunnel support are planned.

## Feedback

Use this repository's Issues to report download or installation problems. Include your OS, processor architecture, and app version. Do not include credentials, account tokens, private tunnel URLs, or sensitive logs.

## Releases

Future version-tag releases build all four desktop targets privately, package only the seven allowlisted installers, generate checksums, and publish the public preview only after all builds succeed. A scoped distribution credential must be configured by the owner before automatic publication is active. No source code or private CI logs are mirrored here.
