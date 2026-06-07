<p align="center">
  <img src="Telegram/Resources/art/sleepygram_1024.png" alt="SleepyGram logo" width="180">
</p>

<h1 align="center">SleepyGram Desktop</h1>

<p align="center">
  A Telegram Desktop fork based on Telegram Desktop 6.8.2 with AyuGram's privacy, history, and customization features kept alive.
</p>

<p align="center">
  <a href="README-RU.md">Русский</a>
  ·
  <a href="https://github.com/slpkbt/SleepyGram/releases">Releases</a>
  ·
  <a href="https://github.com/slpkbt/SleepyGram/issues">Issues</a>
</p>

## Why SleepyGram exists

SleepyGram exists because AyuGram updates have been slow, user ideas from issues have not been actively supported, and the original project appears to have stalled.

The goal is simple: keep the useful AyuGram feature set, move it to current Telegram Desktop releases faster, and treat user feedback as part of the product instead of background noise.

We will be glad to see you among SleepyGram users.

## Features

- Ghost mode and privacy controls
- Message history and anti-recall
- Deleted message and media preservation
- Font and appearance customization
- Streamer mode
- Local Telegram Premium options
- Translator support
- Media preview and quick reaction on force click on macOS
- Extra chat, folder, and interface settings inherited from AyuGram

## Downloads

Release builds will be published on the [Releases](https://github.com/slpkbt/SleepyGram/releases) page.

GitHub Actions also builds CI artifacts:

- `SleepyGram-windows-x64.zip`
- `SleepyGram-linux-x64.tar.xz`
- `SleepyGram-macos-x64.zip`

CI artifacts do not publish auto-update packages.

## App Identity

SleepyGram uses separate application identifiers, executable names, and data directories. It starts as a separate client and does not share an existing AyuGram profile.

- Product name: `SleepyGram Desktop`
- Executable name: `SleepyGram`
- macOS bundle id: `com.sleepygram.desktop`
- Linux app id: `com.sleepygram.desktop`
- Windows app id: `{09F8EFBD-99A0-4326-9A2F-2694574B75CB}`

## Building

Use `.github/workflows/build.yml` to build Windows, Linux, and macOS artifacts.

Preferred Telegram API credential secrets:

- `TDESKTOP_API_ID`
- `TDESKTOP_API_HASH`

The workflow also accepts `AYUGRAM_API_ID` / `AYUGRAM_API_HASH`, `TELEGRAM_API_ID` / `TELEGRAM_API_HASH`, or `API_ID` / `API_HASH`. If no matching secrets are configured, CI falls back to the public credentials documented in `docs/api_credentials.md`.

## Credits

SleepyGram is based on:

- [Telegram Desktop](https://github.com/telegramdesktop/tdesktop)
- [AyuGram Desktop](https://github.com/AyuGram/AyuGramDesktop)

Libraries and third-party components are credited in their original source locations.
