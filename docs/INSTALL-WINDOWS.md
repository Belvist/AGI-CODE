# Установка AGI на Windows

## Скачать

Только официальный установщик:

**[AGI-Setup-0.2.6.exe](https://github.com/Belvist/AGI-CODE/releases/latest/download/AGI-Setup-0.2.6.exe)**

> Не используйте отдельный файл `AGI.exe` без полной папки установки — появится ошибка `ffmpeg.dll`.

## Установка

1. Запустите **AGI-Setup-0.2.6.exe**
2. Следуйте мастеру установки
3. Запустите **AGI** из меню Пуск

## SmartScreen

Windows может показать предупреждение для новых сборок без корпоративной подписи Authenticode.  
Нажмите **Подробнее → Выполнить в любом случае**, если скачали с официальной страницы Releases.

## После установки

1. Установите [LM Studio](https://lmstudio.ai) и включите **Local Server**, **или** задайте ключ OpenRouter в Настройках AGI
2. Нажмите **«Запустить ИИ»** в шапке окна

Лог службы: `%USERPROFILE%\.forgevault\daemon.log`

## Автообновление

Приложение проверяет [latest.yml](https://github.com/Belvist/AGI-CODE/releases/latest/download/latest.yml) и предложит обновление до новой версии.
