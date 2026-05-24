# Публикация на GitHub — ТОЛЬКО без исходников

## Запрещено

- `git push origin main` из полного локального репозитория
- Пуш `packages/`, `scripts/`, workflow-сборок в `Belvist/AGI-CODE`

## Разрешено

1. **Публичная страница:**  
   `.\scripts\push-public-landing-only.ps1 -ExecuteForcePush`

2. **Бинарники релиза (API):**  
   `.\scripts\publish-github-api.ps1 -RepoSlug Belvist/AGI-CODE -Version 0.2.6 -ReplaceAssets`

3. **Удалить старые релизы:**  
   `.\scripts\delete-github-releases.ps1 -RepoSlug Belvist/AGI-CODE -KeepVersions 0.2.6 -DeleteTags`

## Pre-push hook (опционально)

```powershell
Copy-Item scripts\git-hooks\pre-push-no-source .git\hooks\pre-push
```

## Mac DMG

Сборка `.dmg` только на macOS или через **private** репозиторий с workflow `release-mac.yml`.  
На Windows собрать Mac-версию нельзя.

## Подпись (Authenticode / Apple)

Без купленных сертификатов SmartScreen и Gatekeeper показывают предупреждения.  
Для подписи Windows: переменные `CSC_LINK` / `CSC_KEY_PASSWORD`.  
Для macOS: Apple Developer + notarization в `electron-builder`.
