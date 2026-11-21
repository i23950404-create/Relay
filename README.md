# Relay

[English](#english) · [Русский](#русский)

---

## English

Starts a chain of programs (for example, a VPN) before a chosen Windows program — however you open it: from a shortcut, the Start menu, File Explorer, or another application. Works with both classic `.exe` applications and Microsoft Store (MSIX) apps.

### Features

- **Ordered dependency chains** with readiness checks (process launch, local port availability on `127.0.0.1` / `::1`, or internet connectivity).
- **Auto-close with target app**: optionally closes launched helper programs when the main app exits (shared across rules, so a common VPN stays up until the last app using it closes).
- **Elevated steps without repeated UAC prompts** for administrator-protected executables (such as programs installed under `Program Files`).
- **Conditions**: trigger rules only on specific Wi-Fi networks, within a time window, or under a selected power state.
- **System tray & mini-window**: quick access to toggle rules, launch on demand, toggle autostart, or pause all rules temporarily.
- **5 interface languages**: English, Russian, German, French, and Simplified Chinese.
- **Update check**: optional daily check against GitHub Releases (can be disabled in Settings).

### Installation (Windows 10 / 11 x64)

- **MSI installer (recommended)**: download `Relay-<version>-x64.msi` from [Releases](https://github.com/i23950404-create/Relay/releases). Installs Relay to `C:\Program Files\Relay`, adds a Start menu shortcut, and starts the tray app. Uninstalling cleanly removes all system hooks while keeping your rules in `C:\ProgramData\Relay`.
- **Portable**: download `Relay-<version>-x64-portable.zip` from [Releases](https://github.com/i23950404-create/Relay/releases).
- **winget**: `winget install i23950404-create.Relay` *(once published to the winget catalog)*.

> **Verification & SmartScreen:** Every release includes `SHA256SUMS.txt` so you can verify file integrity. The installer is currently unsigned, so Windows SmartScreen may show a warning on first launch — click **More info** → **Run anyway**.

### License

[Relay Freeware License](LICENSE) — free for personal and commercial use of unmodified official builds.

---

## Русский

Запускает цепочку программ (например, VPN) перед выбранной программой в Windows — при **любом** способе её запуска: с ярлыка, из меню «Пуск», Проводника или другой программы. Поддерживаются как обычные программы (`.exe`), так и приложения Microsoft Store (MSIX).

### Основные возможности

- **Цепочки запуска по порядку** с проверкой готовности (появление процесса, открытие локального порта на `127.0.0.1` / `::1` или доступ в интернет).
- **Автозакрытие вместе с программой**: может закрывать запущенные вспомогательные программы после выхода из основной (с общим учётом: общий VPN закроется только после закрытия последней нужной ему программы).
- **Запуск от администратора без постоянного UAC** для защищённых программ (например, установленных в `Program Files`).
- **Условия срабатывания**: только в указанных сетях Wi-Fi, в заданное время или при нужном режиме питания.
- **Значок в трее и мини-окно**: быстрое включение и выключение правил, ручной запуск, автозапуск и режим паузы.
- **5 языков интерфейса**: русский, английский, немецкий, французский и китайский (упрощённый).
- **Проверка обновлений**: раз в день проверяет выход новых версий на GitHub (можно отключить в настройках).

### Установка (Windows 10 / 11 x64)

- **Установщик MSI (рекомендуется)**: скачайте `Relay-<версия>-x64.msi` со страницы [Releases](https://github.com/i23950404-create/Relay/releases). Устанавливает Relay в `C:\Program Files\Relay`, добавляет ярлык в меню «Пуск» и запускает значок в трее. При удалении снимает все системные хуки, сохраняя правила в `C:\ProgramData\Relay`.
- **Портативная версия**: скачайте `Relay-<версия>-x64-portable.zip` со страницы [Releases](https://github.com/i23950404-create/Relay/releases).
- **winget**: `winget install i23950404-create.Relay` *(после публикации пакета в каталоге winget)*.

> **Проверка файлов и SmartScreen:** В каждом выпуске есть файл `SHA256SUMS.txt` для проверки контрольных сумм. Установщик пока без цифровой подписи, поэтому при первом запуске Windows SmartScreen может показать предупреждение — нажмите **Подробнее** → **Выполнить в любом случае**.

### Лицензия

[Relay Freeware License](LICENSE) — бесплатное использование оригинальных официальных сборок в личных и коммерческих целях.
