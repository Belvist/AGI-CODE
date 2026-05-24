<p align="center">
  <img src="https://raw.githubusercontent.com/Belvist/AGI-CODE/main/assets/agi-icon.png" width="96" alt="AGI" />
</p>

<h1 align="center">AGI</h1>

<p align="center">
  <strong>Локальная среда разработки с ИИ на вашем компьютере</strong><br/>
  Редактор, чат, агент — без отправки кода на сторонние серверы по умолчанию.
</p>

<p align="center">
  <a href="https://github.com/Belvist/AGI-CODE/releases/latest"><img src="https://img.shields.io/github/v/release/Belvist/AGI-CODE?label=Release&style=for-the-badge" alt="Release"/></a>
  <img src="https://img.shields.io/badge/platform-Windows%20%7C%20macOS-blue?style=for-the-badge" alt="Platform"/>
  <img src="https://img.shields.io/badge/source-closed-lightgrey?style=for-the-badge" alt="Closed source"/>
</p>

---

## Скачать

| Платформа | Файл | Примечание |
|-----------|------|------------|
| **Windows 10+** | [**AGI-Setup-0.2.7.exe**](https://github.com/Belvist/AGI-CODE/releases/latest/download/AGI-Setup-0.2.7.exe) | Только установщик — **не** скачивайте отдельный `AGI.exe` |
| **macOS 11+** (Apple Silicon) | [**AGI-0.2.7-arm64.dmg**](https://github.com/Belvist/AGI-CODE/releases/latest/download/AGI-0.2.7-arm64.dmg) | ПКМ → **Открыть** при первом запуске |
| **macOS 11+** (Intel) | `AGI-0.2.7-x64.dmg` | На [Releases](https://github.com/Belvist/AGI-CODE/releases/latest), если опубликован |

Автообновление в приложении (Windows): [latest.yml](https://github.com/Belvist/AGI-CODE/releases/latest/download/latest.yml)

---

## Что нужно для работы ИИ

1. **LM Studio** — [lmstudio.ai](https://lmstudio.ai) → загрузите модель → включите **Local Server** (порт 1234), **или**
2. **OpenRouter** — ключ API в **Настройки → Источник моделей** в AGI.

После установки AGI нажмите **«Запустить ИИ»** в шапке окна.

---

## Что нового в v0.2.7

- Автообновления через GitHub Releases  
- Русский интерфейс и лицензия в установщике Windows  
- История чатов, компактная панель редактора, подсветка diff  
- Понятные ошибки LM Studio при переполнении контекста  
- Исправлена кириллица в сообщениях службы (без «кракозябр»)  
- Надёжный запуск встроенной службы на `127.0.0.1:3741`  
- Обновлённые иконки: установщик и иконка приложения разделены  
- Только нужные файлы в релизе — без лишних бинарников  

---

## Установка

### Windows

1. Скачайте **AGI-Setup-0.2.6.exe** по ссылке выше.  
2. Запустите установщик → следуйте мастеру → **Готово**.  
3. Запустите **AGI** из меню Пуск.

> Windows SmartScreen может показать предупреждение для новых сборок без корпоративной подписи. Нажмите **Подробнее → Выполнить в любом случае**, если доверяете источнику (этот репозиторий).

### macOS

1. Скачайте `.dmg` для вашего процессора (M‑series → arm64, Intel → x64).  
2. Откройте образ → перетащите **AGI** в **Programs** (Applications).  
3. Первый запуск: **ПКМ по AGI → Открыть → Открыть** (сборка без подписи Apple Developer).

---

## Безопасность и конфиденциальность

- Исходный код приложения **не публикуется** — здесь только установщики и документация.  
- Служба AGI слушает только **localhost** (`127.0.0.1:3741`).  
- Промпты уходят на **LM Studio / OpenRouter**, которые вы настраиваете сами.

---

## Поддержка

- **Обновления:** [Releases](https://github.com/Belvist/AGI-CODE/releases)  
- **Проблемы с установкой:** убедитесь, что используете **AGI-Setup-*.exe**, а не отдельный exe из архива  
- **Служба не отвечает:** `%USERPROFILE%\.forgevault\daemon.log` (Windows) или `~/.forgevault/daemon.log` (macOS)

---

<p align="center"><sub>© AGI · Belvist · Только официальные сборки с этой страницы Releases</sub></p>
