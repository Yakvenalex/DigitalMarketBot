**DigitalMarketBot** — это учебный проект, представляющий собой пример Telegram-бота для цифрового интернет-магазина, 
разработанный с использованием современных технологий Python.

## Описание

Данный бот демонстрирует функциональность интернет-магазина цифровых товаров в Telegram, включая интеграцию с платёжной 
системой ЮKassa через BotFather. Проект создан в качестве демонстрационного для статьи на Хабре.

## Технологии

В проекте используются следующие технологии:

- **aiogram** 3.15.0 — асинхронный фреймворк для разработки Telegram-ботов.
- **aiosqlite** 0.20.0 — асинхронный драйвер для работы с SQLite.
- **loguru** 0.7.2 — библиотека для продвинутого логирования.
- **pydantic-settings** 2.7.0 — управление настройками с использованием Pydantic.
- **SQLAlchemy** 2.0.35 — SQL-библиотека и ORM для Python.
- **pydantic** >=2.4.1,<2.10 — библиотека для валидации данных и управления настройками.
- **alembic** 1.14.0 — инструмент для управления миграциями базы данных.

## Установка

1. Клонируйте репозиторий:

   ```bash
   git clone https://github.com/Yakvenalex/DigitalMarketBot.git
   ```

2. Перейдите в директорию проекта:

   ```bash
   cd DigitalMarketBot
   ```

3. Создайте и активируйте виртуальное окружение:

   ```bash
   python -m venv venv
   source venv/bin/activate  # Для Windows: venv\Scripts\activate
   ```

4. Получите токен бота через [@BotFather](https://t.me/BotFather).
5. Получите платежный токен ЮКассы через [@BotFather](https://t.me/BotFather) (подойдет тестовый).

6. Установите зависимости:

   ```bash
   pip install -r requirements.txt
   ```

7. Создайте файл `.env` в корне проекта:

   ```
   BOT_TOKEN=ВАШ_ТОКЕН
   ADMIN_IDS=[ADMIN_TG1, ADMIN_TG2, ADMIN_TG3]
   PROVIDER_TOKEN=ТОКЕН_Ю_КАССЫ
   ```

8. Запустите бота:

   ```bash
   python bot/main.py
   ```

## Использование

После запуска бота вы можете взаимодействовать с ним в Telegram. Бот предоставляет функциональность цифрового 
интернет-магазина с возможностью тестовой оплаты через ЮKassa.

### Тестовые данные для оплаты

- **Карта:** 1111 1111 1111 1026
- **Годен до:** 12/26
- **CVC-код:** 000

## Автор

**Алексей Яковенко** [Telegram](https://t.me/yakvenalexx) — разработчик данного учебного проекта.

## Лицензия

Этот проект распространяется под лицензией MIT.

## Демонстрация

**Видео-демка проекта:** [ВИДЕО](https://rutube.ru/video/f57c1617bd03368611ee8aeb44ccb2e5/) — демонстрация всего 
функционала бота в одном видео.

[Ссылка на работающего бота](https://t.me/DigitalMarketAiogramBot) — демонстрация всего 
функционала бота в одном видео.

## Дополнительная информация

Для более подробного изучения кода и архитектуры проекта рекомендуется ознакомиться с исходным кодом и комментариями в 
репозитории.



> **Примечание:** Проект создан в образовательных целях и не предназначен для использования в реальных коммерческих 
> проектах без соответствующей доработки и тестирования.