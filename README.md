# Xray-Checker GitHub Action

This repository contains a GitHub Action that regularly checks Xray configurations using [Xray-Checker](https://github.com/kutovoys/xray-checker).

## Features

- Automatic checks every 5 minutes
- Uses the latest version of xray-checker
- Configurable instance name for metrics
- Manual trigger option with custom arguments

## How to use

1. [Fork](https://github.com/kutovoys/xray-checker-in-actions/fork) this repository
2. Configure repository secrets in your fork:
   - `SUBSCRIPTION_URL`: Your subscription URL
   - `PUSH_URL`: Metrics push URL
   - `INSTANCE`: (Optional) Instance name for metrics (defaults to 'github-actions')

### Setting up secrets

1. Go to your forked repository
2. Click on "Settings" tab
3. In the left sidebar, click on "Secrets and variables" → "Actions"
4. Click "New repository secret"
5. Add the following secrets:
   - Name: `SUBSCRIPTION_URL`
     Value: Your subscription URL
   - Name: `PUSH_URL`
     Value: Your metrics push URL
   - Name: `INSTANCE` (optional)
     Value: Your instance name

### Enabling the Action

The checker will run automatically every 5 minutes after you set up the secrets. You can also run it manually:

1. Go to "Actions" tab in your repository
2. Select "Run xray-checker" workflow
3. Click "Run workflow"

---

# Xray-Checker GitHub Action [RU]

Этот репозиторий содержит GitHub Action для регулярной проверки конфигураций Xray с помощью [Xray-Checker](https://github.com/kutovoys/xray-checker).

## Возможности

- Автоматические проверки каждые 5 минут
- Использование последней версии xray-checker
- Настраиваемое имя инстанса для метрик
- Возможность ручного запуска с пользовательскими аргументами

## Как использовать

1. [Сделайте форк](https://github.com/kutovoys/xray-checker-in-actions/fork) этого репозитория
2. Настройте секреты в вашем форке:
   - `SUBSCRIPTION_URL`: URL вашей подписки
   - `PUSH_URL`: URL для отправки метрик
   - `INSTANCE`: (Опционально) Имя инстанса для метрик (по умолчанию 'github-actions')

### Настройка секретов

1. Перейдите в ваш форк репозитория
2. Нажмите на вкладку "Settings"
3. В левом меню выберите "Secrets and variables" → "Actions"
4. Нажмите "New repository secret"
5. Добавьте следующие секреты:
   - Имя: `SUBSCRIPTION_URL`
     Значение: URL вашей подписки
   - Имя: `PUSH_URL`
     Значение: URL для отправки метрик
   - Имя: `INSTANCE` (опционально)
     Значение: Имя вашего инстанса

### Включение Action

Проверка будет запускаться автоматически каждые 5 минут после настройки секретов. Вы также можете запустить её вручную:

1. Перейдите на вкладку "Actions" в вашем репозитории
2. Выберите воркфлоу "Run xray-checker"
3. Нажмите "Run workflow"
