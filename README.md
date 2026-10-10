# DMeloper's Block Pet — Test Releases

[한국어](README.ko-KR.md) · English

This repository provides builds for checking installation and updates. These are test releases, not official releases.

[Download the latest test build](https://github.com/oup030416/dmelopers-block-pet-test/releases/latest)

## Installation

The versioned `dmelopers-block-pet_*_x64-setup.exe` is the WiX installer. Open Uninstall in its installation folder or use Windows Installed apps to remove it. Data deletion is unchecked by default.

Minimum: x64 Windows 10 22H2 with the September 2023 cumulative update (build 19045.3448), or Windows 11 22H2 with the September 2023 cumulative update (build 22621.2283), or later. Windows 11 24H2 or newer is recommended. Microsoft WebView2 Runtime is required; setup installs it when needed using an internet connection. If that fails, install it from the Microsoft page opened by the app.

Close the app normally before running the EXE. If installation is interrupted, run the same installer again to repair the program files. The installer can roll back failed MSI changes; it does not automatically restore user data.

Test builds use the requested app and installer version, a separate test signature and update source, and data stored separately from official installations.

## Updates

Install an earlier test version, then check for a newer version in Settings to test the signed update. The app and installer use the version shown in the release. Earlier WiX-suffixed installers use different download filenames; remove those installations with data deletion unchecked, then install this build.

Test builds can install a higher version after you request an update. Files in ordinary versioned test releases, including v1.0.0, may be replaced. To install replacement files at the same version, download them again and reinstall manually.

Read each release's description before installing. Test releases do not change official installation identities or update sources.

## Download Warnings

Compare the downloaded files with the release's current SHA-256 checksums. In PowerShell, use `Get-FileHash -Algorithm SHA256 -LiteralPath '<downloaded file>'`. A matching hash confirms matching bytes; it does not establish safety or the publisher's identity.

These GitHub installers have no Authenticode signature, so Windows may show an unknown publisher. The accompanying `.sig` file is a separate update signature. If a hash differs or security software reports malware, do not run the file.

Test results do not establish official release readiness or antivirus acceptance. Unperformed checks remain unverified.

## About This Repository

This repository contains the test guide and badge generation code. The publisher refreshes badges after deployment; there is no scheduled refresh. Older immutable releases remain in the former repository.

The [official repository](https://github.com/d-meloper/dmelopers-block-pet) is separate. Official GitHub updates start at the user's request; Windows manages Store updates.

Not an official Minecraft product. Not approved by or associated with Mojang or Microsoft.
