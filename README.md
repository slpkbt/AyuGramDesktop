# SleepyGram Desktop

SleepyGram Desktop is a Telegram Desktop fork based on Telegram Desktop 6.8.2 stable with the extended feature set kept in place.

## Why SleepyGram exists

SleepyGram exists because AyuGram updates have been slow, user ideas from issues have not been actively supported, and the original project appears to have stalled. This fork is meant to keep the AyuGram feature set moving on top of current Telegram Desktop releases.

We will be glad to see you among SleepyGram users.

## Features

- Full ghost mode
- Message history
- Anti-recall
- Font customization
- Streamer mode
- Local Telegram Premium
- Translator
- Media preview and quick reaction on force click on macOS
- Enhanced appearance settings

## Identity

SleepyGram uses its own application identifiers, executable name, and data directories. It starts as a separate client and does not share an existing profile.

- Product name: `SleepyGram Desktop`
- Executable name: `SleepyGram`
- macOS bundle id: `com.sleepygram.desktop`
- Linux app id: `com.sleepygram.desktop`
- Windows app id: `{09F8EFBD-99A0-4326-9A2F-2694574B75CB}`

## Build

Use the workflow in `.github/workflows/build.yml` to build Windows, Linux, and macOS artifacts. The workflow requires API credentials. Preferred secret names:

- `TDESKTOP_API_ID`
- `TDESKTOP_API_HASH`

For temporary AyuGram reuse, the workflow also accepts `AYUGRAM_API_ID` / `AYUGRAM_API_HASH`, `TELEGRAM_API_ID` / `TELEGRAM_API_HASH`, or `API_ID` / `API_HASH`. If no matching secrets are configured, CI falls back to the public credentials documented in `docs/api_credentials.md`.

Artifacts produced by CI:

- `SleepyGram-windows-x64.zip`
- `SleepyGram-linux-x64.tar.xz`
- `SleepyGram-macos-x64.zip`

Auto-update packaging is disabled for CI artifacts.

## Credits

SleepyGram is based on:

- [Telegram Desktop](https://github.com/telegramdesktop/tdesktop)
- [AyuGram Desktop](https://github.com/AyuGram/AyuGramDesktop)

Libraries and third-party components are credited in their original source locations.
