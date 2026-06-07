# Contributing

This document describes how you can contribute to SleepyGram Desktop.

## What contributions are accepted

We accept focused bug fixes, build fixes, documentation improvements, and feature work that fits the SleepyGram direction: keeping useful AyuGram-style features working on top of current Telegram Desktop releases.

Feature ideas are welcome in [issues](https://github.com/slpkbt/SleepyGram/issues). Keep requests concrete and explain the use case.

## Build instructions

See the [build documentation](https://github.com/slpkbt/SleepyGram/blob/dev/docs) for platform-specific setup.

## Upstreams

SleepyGram tracks two upstreams:

- [Telegram Desktop](https://github.com/telegramdesktop/tdesktop) for the base client
- [AyuGram Desktop](https://github.com/AyuGram/AyuGramDesktop) for the feature set inherited by SleepyGram

When syncing manually, keep changes split clearly:

- Telegram Desktop version syncs
- AyuGram feature fixes
- SleepyGram branding and product changes

## Pull requests

- Keep pull requests focused on a single issue or feature.
- Do not mix code changes with unrelated whitespace cleanup.
- Keep user-facing strings polished and consistent with the surrounding UI.
- Do not rename internal `Ayu*` code just for branding. That creates risk without improving the product.
- Test the changed area before opening a pull request.

## Commit messages

Write commit messages that explain what changed and why. If a commit fixes an issue, reference it with `Fix #123`.

[closing-issues-via-commit-messages]: https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/linking-a-pull-request-to-an-issue
