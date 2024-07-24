[![Тесты Playwright](https://github.com/raptatinha/tau-advanced-playwright/actions/workflows/playwright.yml/badge.svg)](https://github.com/raptatinha/tau-advanced-playwright/actions/workflows/playwright.yml)

# Продвинутый Playwright

Привет 👋🏽!

Добро пожаловать на курс "Продвинутый Playwright" от [Ренаты Андраде](https://testingwithrenata.com/) для [Университета Автоматизации Тестирования](https://testautomationu.applitools.com/). Если вы новичок в Playwright, я приглашаю вас ознакомиться с курсом [Введение в Playwright](https://testautomationu.applitools.com/instructors/renata_andrade.html).

## Зависимости

- Playwright v1.35.1
- Node v20.3.0
- npm v9.6.5
- VSCode Версия: 1.79.1 (Универсальная)
- Applitools v1.17.5

> Предварительные требования:
- [Установка Node](https://nodejs.dev/en/learn/how-to-install-nodejs/)
- [Установка VS Code](https://code.visualstudio.com/learn/get-started/basics)
- [Установка iTerm](https://iterm2.com/documentation-one-page.html)

## Форк и клонирование проекта

1. Скопируйте URL проекта `https://github.com/raptatinha/tau-advanced-playwright.git`;
1. Сделайте форк проекта, следуя [инструкциям GitHub](https://docs.github.com/en/get-started/quickstart/fork-a-repo) - (используйте параметр --clone=true);
1. Перейдите в форкнутый проект `cd tau-advanced-playwright`

ПРИМЕЧАНИЕ: Не забудьте добавить секреты и переменные в ваш локальный репозиторий.

## Установка проекта

ВАЖНО: Создайте ваш файл [.env](.env) следуя примеру [.env.example](.env.example). Единственный параметр, который вам нужно обновить, это `APPLITOOLS_API_KEY` для ваших учетных данных.

В вашем терминале введите:

1. `npm i`

## Запуск проекта
Обратите внимание на [package.json](package.json) - скрипты для более подробной информации. Тесты используют https://demoqa.com/

- `npm run test-ui-c` запускает все тесты на chromium (кроме авторизации)
- `npm run test-ui-auth-admin` запускает profile-stored-auth-multi-role-admin.spec.ts
- `npm run test-ui-auth-user` запускает profile-stored-auth-multi-role-user.spec.ts
- `npm run test-ui-auth` запускает profile-stored-auth-multi-role-example.spec.ts (тест завершится неудачно из-за ограничений приложения)
- `npm run test-vrt` запускает visual-regression.spec.ts - тестирование визуальной регрессии с помощью applitools

## Содержание курса:
### Глава 1: Оптимизация аутентификации
- Обычная аутентификация с использованием page objects;
- Сохраненная аутентификация с использованием global-setup через UI;
- Сохраненная аутентификация для нескольких пользователей;
- Продвинутая - аутентификация через API запрос;
### Глава 2: Динамические Page Objects & Fixtures
- Файл hooks для повторно используемых созданий page object
- URL builder для динамического создания URL
- Файл fixtures для повторно используемых потоков
### Глава 3: Взаимодействие с API
- APIRequestContext
- HTTP методы, опции запроса, URL запроса
- Как идентифицировать API вызов и использовать swagger
- Динамическое выполнение запроса
- Обработка ошибок
- Повторное использование
### Глава 4: Управление данными
- Через .env файлы
- Через JSON
- Через API
- Через мок данные
- Через CSV - https://playwright.dev/docs/test-parameterize#create-tests-via-a-csv-file
### Глава 5: Визуальная регрессия с Applitools
- Реализация теста визуальной регрессии
- Использование различных настроек проверки
- Интерпретация результатов
### Глава 6: Непрерывная интеграция & Наблюдаемость
- Github Actions
- Файл yml
- Интеграция с Slack
- Стратегия параллелизации & Sharding

___

💡 Поделитесь в LinkedIn чем-то интересным, что вы узнали! Не забудьте отметить меня [Ренату Андраде](https://www.linkedin.com/in/raptatinha/).

💜 Если у вас есть вопросы, не стесняйтесь задавать их на [github](https://github.com/raptatinha/tau-advanced-playwright/issues).

Счастливого тестирования 🎭
