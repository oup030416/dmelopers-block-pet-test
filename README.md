# DMeloper's Block Pet — Test Releases

[한국어](README.ko-KR.md) · English

This repository provides builds for checking installation and updates. These are test releases, not official releases.

[Download test builds](https://github.com/oup030416/dmelopers-block-pet-test/releases)

## Installation

The versioned `dmelopers-block-pet_*_x64-setup.exe` is the WiX installer. Open Uninstall in its installation folder or use Windows Installed apps to remove it. Data deletion is unchecked by default.

Windows 11 24H2 or newer (x64) and Microsoft WebView2 Runtime are required. If WebView2 is missing, install it from the Microsoft page opened by the app or installer.

Close the app normally before running the EXE. If installation is interrupted, run the same installer again to repair the program files. The installer can roll back failed MSI changes; it does not automatically restore user data.

Ordinary test builds use a separate test signature and store their data separately from official installations. A release marked as a test of the official binary keeps that binary's official update source and shared Saved Games data; uploading it here does not change its behavior.

## Updates

Install the current 1.0.0 installer to test the signed update to 1.0.1 from Settings. Earlier WiX-suffixed installers use different download filenames; remove those installations with data deletion unchecked, then install this build.

Test builds can install a higher version after you request an update. Files in ordinary versioned test releases, including v1.0.0, may be replaced. To install replacement files at the same version, download them again and reinstall manually.

Official-binary candidates use separate prerelease tags and retain their exact files. They do not update the test feed or badges. Read each release's description before installing.

## Download Warnings

Compare the downloaded files with the release's current SHA-256 checksums. In PowerShell, use `Get-FileHash -Algorithm SHA256 -LiteralPath '<downloaded file>'`. A matching hash confirms matching bytes; it does not establish safety or the publisher's identity.

These GitHub installers have no Authenticode signature, so Windows may show an unknown publisher. The accompanying `.sig` file is a separate update signature. If a hash differs or security software reports malware, do not run the file.

Test results do not establish official release readiness or antivirus acceptance. Unperformed checks remain unverified.

## About This Repository

This repository contains the test guide and badge generation code. The publisher refreshes badges after deployment; there is no scheduled refresh. Older immutable releases remain in the former repository.

The [official repository](https://github.com/d-meloper/dmelopers-block-pet) is separate and may remain private before launch. Official GitHub updates start at the user's request; Windows manages Store updates.

Not an official Minecraft product. Not approved by or associated with Mojang or Microsoft.
