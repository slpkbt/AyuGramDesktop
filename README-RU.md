<p align="center">
  <img src="Telegram/Resources/art/sleepygram_1024.png" alt="SleepyGram logo" width="180">
</p>

<h1 align="center">SleepyGram Desktop</h1>

<p align="center">
  Форк Telegram Desktop 6.8.2 с сохраненными privacy-функциями, историей сообщений и кастомизацией AyuGram.
</p>

<p align="center">
  <a href="README.md">English</a>
  ·
  <a href="https://github.com/slpkbt/SleepyGram/releases">Releases</a>
  ·
  <a href="https://github.com/slpkbt/SleepyGram/issues">Issues</a>
</p>

## Почему существует SleepyGram

SleepyGram появился потому, что AyuGram медленно обновляется, идеи пользователей из issues почти не получают поддержки, а сам проект выглядит заброшенным.

Цель простая: сохранить полезные функции AyuGram, быстрее переносить их на актуальные версии Telegram Desktop и относиться к фидбеку пользователей как к части продукта, а не как к шуму на фоне.

Буду рад видеть вас в числе пользователей SleepyGram!

## Функции

- Ghost Mode и privacy-настройки
- История сообщений и anti-recall
- Сохранение удаленных сообщений и медиа
- Кастомизация шрифтов и внешнего вида
- Streamer Mode
- Локальные опции Telegram Premium
- Переводчик
- Превью медиа и быстрая реакция при force click на macOS
- Дополнительные настройки чатов, папок и интерфейса из AyuGram

## Скачать

Готовые сборки будут публиковаться на странице [Releases](https://github.com/slpkbt/SleepyGram/releases).

GitHub Actions также собирает CI artifacts:

- `SleepyGram-windows-x64.zip`
- `SleepyGram-linux-x64.tar.xz`
- `SleepyGram-macos-x64.zip`

CI artifacts не публикуют auto-update packages.

## App Identity

SleepyGram использует отдельные application ids, имя бинаря и директории данных. Клиент стартует отдельно и не использует существующий профиль AyuGram.

- Product name: `SleepyGram Desktop`
- Executable name: `SleepyGram`
- macOS bundle id: `com.sleepygram.desktop`
- Linux app id: `com.sleepygram.desktop`
- Windows app id: `{09F8EFBD-99A0-4326-9A2F-2694574B75CB}`

## Сборка

Для сборки Windows, Linux и macOS artifacts используется `.github/workflows/build.yml`.

Основные Telegram API credential secrets:

- `TDESKTOP_API_ID`
- `TDESKTOP_API_HASH`

Workflow также принимает `AYUGRAM_API_ID` / `AYUGRAM_API_HASH`, `TELEGRAM_API_ID` / `TELEGRAM_API_HASH` или `API_ID` / `API_HASH`. Если таких secrets нет, CI использует публичные credentials из `docs/api_credentials.md`.

## Credits

SleepyGram основан на:

- [Telegram Desktop](https://github.com/telegramdesktop/tdesktop)
- [AyuGram Desktop](https://github.com/AyuGram/AyuGramDesktop)

Библиотеки и сторонние компоненты указаны в их исходных местах.
