# Установка AGI на macOS

## Требования

- macOS 11 (Big Sur) или новее
- [LM Studio](https://lmstudio.ai) с включённым **Local Server**, **или** ключ [OpenRouter](https://openrouter.ai)

## Скачать

1. Откройте [Releases](https://github.com/Belvist/AGI-CODE/releases/latest)
2. Скачайте:
   - **Apple Silicon (M1/M2/M3):** `AGI-0.2.6-arm64.dmg`
   - **Intel Mac:** `AGI-0.2.6-x64.dmg` (если опубликован)

## Установка

1. Откройте `.dmg`
2. Перетащите **AGI** в папку **Programs** (Applications)
3. Запустите AGI из Applications

## Gatekeeper (первая загрузка)

Сборка не подписана сертификатом Apple Developer. При блокировке:

- **ПКМ** по AGI → **Открыть** → подтвердите **Открыть**

Или в Terminal:

```bash
xattr -dr com.apple.quarantine /Applications/AGI.app
```

## После установки

1. Запустите **LM Studio** → загрузите модель → **Local Server** (порт 1234)
2. В AGI: **Настройки** → источник **LM Studio** или **OpenRouter**
3. Нажмите **«Запустить ИИ»** в шапке

Лог службы: `~/.forgevault/daemon.log`
