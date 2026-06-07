# SleepyGram Desktop

[ English  |  [Русский](README-RU.md) ]

SleepyGram Desktop - форк Telegram Desktop 6.8.2 stable с сохраненным расширенным набором функций.

## Почему существует SleepyGram

SleepyGram появился потому, что AyuGram медленно обновляется, идеи пользователей из issues почти не получают поддержки, а сам проект выглядит заброшенным. Цель SleepyGram - сохранить функции AyuGram и быстрее переносить их на актуальные версии Telegram Desktop.

Буду рад видеть вас в числе пользователей SleepyGram!

## Функции

- Полный Ghost Mode
- История сообщений
- Anti-recall
- Кастомизация шрифтов
- Streamer Mode
- Локальный Telegram Premium
- Переводчик
- Превью медиа и быстрая реакция при force click на macOS
- Расширенные настройки внешнего вида

## Identity

SleepyGram использует отдельные application ids, имя бинаря и директории данных. Клиент стартует отдельно и не использует существующий профиль.

- Product name: `SleepyGram Desktop`
- Executable name: `SleepyGram`
- macOS bundle id: `com.sleepygram.desktop`
- Linux app id: `com.sleepygram.desktop`
- Windows app id: `{09F8EFBD-99A0-4326-9A2F-2694574B75CB}`

## Сборка

GitHub Actions workflow лежит в `.github/workflows/build.yml` и собирает Windows, Linux и macOS artifacts. Для сборки нужны API credentials. Основные имена secrets:

- `TDESKTOP_API_ID`
- `TDESKTOP_API_HASH`

Для временного reuse AyuGram workflow также принимает `AYUGRAM_API_ID` / `AYUGRAM_API_HASH`, `TELEGRAM_API_ID` / `TELEGRAM_API_HASH` или `API_ID` / `API_HASH`. Если таких secrets нет, CI использует публичные credentials из `docs/api_credentials.md`.

Artifacts:

- `SleepyGram-windows-x64.zip`
- `SleepyGram-linux-x64.tar.xz`
- `SleepyGram-macos-x64.zip`

Auto-update в CI artifacts отключен.

## Credits

SleepyGram основан на:

- [Telegram Desktop](https://github.com/telegramdesktop/tdesktop)
- [AyuGram Desktop](https://github.com/AyuGram/AyuGramDesktop)
