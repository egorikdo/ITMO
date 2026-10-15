# Источники и результаты обработки

Исходные лабораторные CandyGoose использованы с разрешения автора (со слов составителя). Это не утверждение об авторстве решений составителем.

| Семестр | Дисциплина | Сохранённые файлы (без README) | Репозиторий |
|---:|---|---:|---|
| 1 | Программирование | 65 | [Источник](https://github.com/CandyGoose/Programming_1_term_SE) |
| 1 | Информатика | 33 | [Источник](https://github.com/CandyGoose/Informatic_SE) |
| 2 | Программирование | 325 | [Источник](https://github.com/CandyGoose/Programming_2_term_SE) |
| 2 | Базы данных | 20 | [Источник](https://github.com/CandyGoose/Database_SE) |
| 2 | Основы профессиональной деятельности | 321 | [Источник](https://github.com/CandyGoose/OPD_web) |
| 3 | Языки программирования | 44 | [Источник](https://github.com/CandyGoose/Programming_languages) |
| 3 | Веб-программирование | 97 | [Источник](https://github.com/CandyGoose/Web_programming_SE) |
| 4 | Математическая статистика | 6 | [Источник](https://github.com/CandyGoose/Mathematical_statistics) |
| 4 | Архитектура компьютера | 24 | [Источник](https://github.com/CandyGoose/Computer_architecture) |
| 4 | Методы оптимизации | 10 | [Источник](https://github.com/CandyGoose/Optimization_methods) |
| 4 | Основы программной инженерии | 264 | [Источник](https://github.com/CandyGoose/Fundamentals_of_SE) |
| 4 | Вычислительная математика | 8 | [Источник](https://github.com/CandyGoose/Computational_math) |
| 4 | Программный проект по физике | 25 | [Источник](https://github.com/CandyGoose/Circuits_constructor) |
| 5 | Системы искусственного интеллекта | 18 | [Источник](https://github.com/CandyGoose/Artificial_intelligence_systems) |
| 5 | Операционные системы | 303 | [Источник](https://github.com/CandyGoose/Operating_systems) |
| 5 | Мультимедиа: визуализация аудио | 5 | [Источник](https://github.com/CandyGoose/Audio_visualization) |
| 5 | Разработка веб-приложений | 194 | [Источник](https://github.com/CandyGoose/Web_application_development) |
| 6 | Разработка мультимедийных приложений | 8 | [Источник](https://github.com/CandyGoose/Multimedia_application_development) |
| 6 | Разработка мобильных приложений | 108 | [Источник](https://github.com/CandyGoose/Mobile_application_development) |
| 6 | Теория систем | 6 | [Источник](https://github.com/CandyGoose/Theory_of_systems) |
| 6 | Нейротехнологии и аффективные вычисления | 7 | [Источник](https://github.com/CandyGoose/Neurotechnology_and_afficient_computing) |
| 6 | Разработка на игровых движках | 1410 | [Источник](https://github.com/CandyGoose/Introduction_to_working_with_game_engines) |
| 7 | Интеллектуальная обработка экспериментальных данных | 5 | [Источник](https://github.com/CandyGoose/Intelligent_processing_of_experimental_data) |
| 7 | Работа с нейроинтерфейсами | 4 | [Источник](https://github.com/CandyGoose/Working_with_neural_interfaces) |
| 7 | Моделирование | 3 | [Источник](https://github.com/CandyGoose/Modeling) |
| 7 | Нейротехнологии на основе ЭЭГ | 33 | [Источник](https://github.com/CandyGoose/Neurotechnologies_based_on_electroencephalography) |
| 7 | Разработка приложений виртуальной реальности | 857 | [Источник](https://github.com/CandyGoose/Virtual_reality_application_development) |

## Удалено

- Удалено файлов и результатов избыточной документации: **621** (включая JavaDoc, файлы `.github`, TMP Examples & Extras).
- Удалены технические метаданные Finder и случайные бинарные/компилированные артефакты.
- Дополнительные PDF/отчёты были исключены ещё на предыдущем этапе.

## Ограничения воспроизводимости

- В исходном архиве **отсутствует `JWTUtils.java`** в `semester-03/web-programming/lab4/backend`: ранний фильтр исключил файл как потенциально содержащий секрет. Модуль может не скомпилироваться без безопасной реализации этого класса.
- В Unity-проектах не было некоторых `ProjectSettings.asset` и бинарных ассетов. Полное воспроизведение сцен не гарантируется.
- Проекты по аффективным вычислениям и ряд других ноутбуков требуют внешних Kaggle/Google Drive-датасетов, библиотек и обученных моделей.
- Данные ЭЭГ `.csv` сохранены как входные данные к ноутбукам; их происхождение и разрешение на публикацию должны быть отдельно подтверждены, если эти измерения содержат персональную информацию.
- Наборы значений `postgres/postgres` в учебных конфигурациях — демонстрационные. Для реальных сервисов необходимо задать безопасные секреты и собственное окружение.
- В `semester-06/mobile-apps/user-service` фиксированный JWT-ключ заменён на обязательную переменную окружения `JWT_SECRET`. В `semester-06/affective-computing/project/main.py` токен бота читается из `BOT_TOKEN`.
- Авторские уведомления в исходном коде и файлах лицензий сторонних компонентов сохранены.
- Запуск каждого из 27 проектов не выполнялся; проверены структура, форматы некоторых файлов, ссылки навигации и базовые риски.

## Исключённые дисциплины

- 5-й семестр: **Биометрия и нейротехнологии** — в полученной отфильтрованной копии не оказалось программного кода.
- 7-й семестр: **Визуализация данных** — сохранились в основном материалы Power BI / DataLens / Google Sheets, без локального проекта с кодом.
- Восьмой семестр и факультативы не включались.
