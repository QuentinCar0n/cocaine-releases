# Cocaine releases

Cocaine is a macOS menu bar app that keeps your Mac awake for a set time, with an optional mouse and trackpad scroll reverser. This repository only hosts the release zips; the source is not public. The current version is 1.3 (October 2026), and installed copies update themselves from this repository's releases.

## At a glance

| | |
| --- | --- |
| What | Menu bar keep-awake app for macOS, with an optional scroll reverser |
| Current version | [1.3](https://github.com/QuentinCar0n/cocaine-releases/releases/tag/v1.3), released 2026-10-09 |
| Download | `Cocaine-<version>.zip` from [Releases](https://github.com/QuentinCar0n/cocaine-releases/releases/latest) |
| Platform | macOS |
| Updates | Automatic: the app checks this repository's releases once a day |
| Signing | Not notarized by Apple (right-click, Open on first launch) |
| Source | Not public. This repository holds release builds only |
| Homebrew | No cask yet |

## Features

- **Keep the Mac awake for a set time.** Turn it on from the menu bar and your Mac stays awake until the time runs out.
- **Optional scroll reverser.** Reverse the scroll direction for a mouse and a trackpad.
- **Self-updating.** Installed copies check this repository once a day and install new versions on their own (from 1.3 on).

## Install

1. Download the latest `Cocaine-<version>.zip` from [Releases](https://github.com/QuentinCar0n/cocaine-releases/releases/latest).
2. Unzip it and move `Cocaine.app` to Applications.
3. The app is not notarized, so right-click it and choose Open the first time.

There's no Homebrew cask for Cocaine. The author's [Homebrew tap](https://github.com/QuentinCar0n/homebrew-tap) currently holds only MultiClaude.

## How updates work

Cocaine polls the [releases of this repository](https://github.com/QuentinCar0n/cocaine-releases/releases) once a day. When a newer release is published, the app downloads its zip and updates itself.

The release zips live in this public repository because the source repository is private, and GitHub hides a private repository's releases from apps that check without an account. That's why version 1.2 could never see an update. If you run 1.2, install 1.3 once by hand; every later version arrives automatically.

## Versions

| Version | Date | Notes |
| --- | --- | --- |
| [1.3](https://github.com/QuentinCar0n/cocaine-releases/releases/tag/v1.3) | 2026-10-09 | Updates now come from this public repository. Copies on 1.2 need one manual install of 1.3 |

## FAQ

**What is Cocaine for Mac?**
A menu bar app that keeps your Mac awake for a set time, with an optional mouse and trackpad scroll reverser. It's distributed as a zip from this repository.

**Is Cocaine an alternative to Caffeine, Amphetamine or Caffeinated?**
It does the same core job as those apps: keep the Mac from sleeping for a while, from the menu bar. It also includes an optional scroll reverser for a mouse and a trackpad. Unlike Amphetamine, which is on the Mac App Store, Cocaine is downloaded from GitHub and isn't notarized.

**How is it different from the built-in `caffeinate` command?**
`caffeinate` ships with macOS and runs in Terminal (for example `caffeinate -d -t 3600` keeps the display awake for an hour). Cocaine does the same kind of thing from a menu bar icon, without a terminal.

**Is Cocaine open source?**
No. The source is not public. This repository only holds release builds.

**Is Cocaine free?**
The release zips are free to download from this repository.

**How do I update Cocaine?**
You don't need to: it checks this repository once a day and updates itself. The one exception is version 1.2, which can't see updates; install 1.3 once by hand.

**macOS says Cocaine can't be opened because Apple cannot check it. What do I do?**
The app isn't notarized. Right-click `Cocaine.app` in Applications and choose Open, then confirm. You only need to do this once.

**Can I install Cocaine with Homebrew?**
Not yet. There's no Cocaine cask in [QuentinCar0n/homebrew-tap](https://github.com/QuentinCar0n/homebrew-tap).

**Which macOS versions does Cocaine support?**
The release notes don't state a minimum version.

## Documentation

- [Releases](https://github.com/QuentinCar0n/cocaine-releases/releases): every version with its notes and zip
- [llms.txt](llms.txt): a short index of this repository for language models

## Related projects

- [MultiClaude](https://github.com/QuentinCar0n/multiclaude): menu bar app to run several Claude desktop accounts on one Mac
- [QuentinCar0n Homebrew tap](https://github.com/QuentinCar0n/homebrew-tap): Homebrew casks for the author's macOS apps
