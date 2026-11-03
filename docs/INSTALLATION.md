# Installing Ethos

[← Back to Ethos downloads](../README.md#download-ethos)

Start with **Ethos Home** to choose, install, open and update the apps you want. Individual app installers are also available on the [download page](../README.md#download-ethos).

## macOS

**Supported build:** Apple Silicon, macOS 11 or later.

1. Download the `.dmg` for Ethos Home or your chosen app.
2. Open the disk image and drag the app to **Applications**.
3. These preview builds are not yet notarized by Apple. For the first launch, right-click the app, choose **Open**, then **Open** again.

## Windows

**Supported build:** 64-bit Windows (x64).

1. Download the `.msi` for Ethos Home or your chosen app.
2. Run the installer. It installs for the current user and does not need administrator rights.
3. These preview builds are not yet signed with a Windows certificate. If Windows SmartScreen identifies an unknown publisher, choose **More info → Run anyway**.

## Check your download

The latest release includes [SHA256SUMS.txt](https://github.com/ssharaf-dot/ethos-releases/releases/latest/download/SHA256SUMS.txt), listing each file’s SHA-256. Ethos Home checks apps against their published SHA-256 before installation.

**macOS — Terminal**

```sh
shasum -a 256 ~/Downloads/Ethos-Home-macOS.dmg
```

**Windows — PowerShell**

```powershell
Get-FileHash "$HOME\Downloads\Ethos-Home-Windows.msi" -Algorithm SHA256
```

Compare the resulting value with the entry for the same file in `SHA256SUMS.txt`. For a different app, replace the filename in the command with the one you downloaded.

## Release information

The [release notes](https://github.com/ssharaf-dot/ethos-releases/releases) contain version-specific changes and installation details. Report a reproducible problem through this repository’s [issues](https://github.com/ssharaf-dot/ethos-releases/issues), including your operating system, app name and version, and the steps that led to it.

[Ethos Technologies](https://www.ethostechnologies.si) · [Credits and licensing](../CREDITS.md)
