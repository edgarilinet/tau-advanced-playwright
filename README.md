[![Тесты драматурга](https://github.com/raptatinha/tau-advanced-playwright/actions/workflows/playwright.yml/badge.svg)](https://github.com/raptatinha/tau-advanced -playwright/actions/workflows/playwright.yml)

#Продвинутый драматург

Привет 👋🏽!

Добро пожаловать на курс «Продвинутый драматург» [Ренаты Андраде] (https://testingwithrenata.com/) для [Университета автоматизации тестирования] (https://testautomationu.applitools.com/).
Если вы новичок в драматурге, я приглашаю вас посмотреть курс [Введение в драматургию](https://testautomationu.applitools.com/instructors/renata_andrade.html).

## Зависимости

- Драматург v1.35.1
- Нода v20.3.0
- НПМ v9.6.5
- Версия VSCode: 1.79.1 (универсальная)
- Приложения v1.17.5

> Предварительные требования:
- [Настройка узла](https://nodejs.dev/en/learn/how-to-install-nodejs/)
- [Настройка VS Code](https://code.visualstudio.com/learn/get-started/basics)
- [настройка iTerm](https://iterm2.com/documentation-one-page.html)

## Форкнуть и клонировать проект

1. Скопируйте URL-адрес проекта https://github.com/raptatinha/tau-advanced-playwright.git;
1. Форкните проект, следуя [инструкциям GitHub](https://docs.github.com/en/get-started/quickstart/fork-a-repo) — (используйте параметр --clone=true);
1. Получите доступ к разветвленному проекту `cd tau-advanced-playwright`.

ПРИМЕЧАНИЕ. Не забудьте добавить секреты и переменные в локальный репозиторий.

## Установите проект

ВАЖНО: Создайте файл [.env](.env) после [.env.example](.env.example). `APPLITOOLS_API_KEY` — единственный параметр, который вам нужно будет обновить в соответствии с вашими учетными данными.

На своем терминале введите:

1. `нпм я`

## Запускаем проект
Подробнее см. в [package.json](package.json) — скриптах.
Тесты проводятся с использованием https://demoqa.com/.

- `npm run test-ui-c` запускает все тесты на хроме (кроме аутентификации)
- `npm run test-ui-auth-admin` запускает Profile-stored-auth-multi-role-admin.spec.ts
- `npm run test-ui-auth-user` запускает Profile-stored-auth-multi-role-user.spec.ts
- `npm run test-ui-auth` запускает Profile-stored-auth-multi-role-example.spec.ts (тест завершится неудачно из-за ограничений приложения)
- `npm run test-vrt` запускает Visual-reгрессия.spec.ts - визуальное регрессионное тестирование с помощью applitools

## Содержание курса:
### Глава 1. Оптимизация аутентификации
- Регулярная аутентификация с объектами страницы;
- Сохраненная аутентификация с глобальной настройкой через пользовательский интерфейс;
- Сохраненная аутентификация для нескольких пользователей;
- Расширенный - авторизация через запрос API;
### Глава 2: Объекты и приспособления динамических страниц
- Файл хуков для создания повторно используемых объектов страницы.
- Конструктор URL-адресов для создания динамических URL-адресов
- Файл фиксов для многоразовых потоков.
### Глава 3. Взаимодействие с API
- Контекст APIRequestContext
- Методы HTTP, параметры запроса, URL-адрес запроса.
- Как идентифицировать вызов API и использовать чванство
- Динамическое выполнение запроса
- Обработка ошибок
- Многоразовое использование
### Глава 4: Управление данными
- Через файлы.env
-Через JSON
- Через API
- Через фиктивные данные
- Через CSV - https://playwright.dev/docs/test-parameterize#create-tests-via-a-csv-file
### Глава 5. Визуальная регрессия с помощью Applitools
- Реализация визуального регрессионного теста.
- Использование различных настроек проверки
- Интерпретация результатов
### Глава 6: Непрерывная интеграция и наблюдаемость
- Действия Гитхаба
- YML-файл
- Слабая интеграция
- Стратегия распараллеливания и шардинг

___

💡 Поделитесь в LinkedIn чем-то интересным, что вы узнали! Не забудьте отметить меня [Ренату Андраде](https://www.linkedin.com/in/raptatinha/).

💜 Если у вас есть вопросы, задавайте их на [github](https://github.com/raptatinha/tau-advanced-playwright/issues).

Приятного тестирования 🎭
