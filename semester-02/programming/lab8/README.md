# Лабораторная №8 · GUI

> **Программирование** · 2-й семестр · `ITMO / Нейротехнологии и программирование`

**Технологии:** Java · Maven

## Задача

1. Интерфейс должен быть реализован с помощью библиотеки JavaFX
2. Графический интерфейс клиентской части должен поддерживать `русский`, `румынский`, `венгерский` и `английский (Индия)` языки / локали. Должно обеспечиваться корректное отображение чисел, даты и времени в соответстии с локалью. Переключение языков должно происходить без перезапуска приложения. Локализованные ресурсы должны храниться в `классе`.
Доработать программу из [лабораторной работы №7](https://github.com/CandyGoose/Programming_2_term_SE/tree/main/lab7) следующим образом:
Заменить консольный клиент на клиент с графическим интерфейсом пользователя(GUI).
В функционал клиента должно входить:
Необходимо реализовать многопоточную обработку запросов.
1. Окно с авторизацией/регистрацией.
2. Отображение текущего пользователя.
3. Таблица, отображающая все объекты из коллекции
1. Каждое поле объекта - отдельная колонка таблицы.
2. Строки таблицы можно фильтровать/сортировать по значениям любой из колонок. Сортировку и фильтрацию значений столбцов реализовать с помощью Streams API.
4. Поддержка всех команд из предыдущих лабораторных работ.
5. Область, визуализирующую объекты коллекции
1. Объекты должны быть нарисованы с помощью графических примитивов с использованием Graphics, Canvas или аналогичных средств графической библиотеки.
2. При визуализации использовать данные о координатах и размерах объекта.
3. Объекты от разных пользователей должны быть нарисованы разными цветами.
4. При нажатии на объект должна выводиться информация об этом объекте.
5. При добавлении/удалении/изменении объекта, он должен **автоматически** появиться/исчезнуть/измениться  на области как владельца, так и всех других клиентов.

_Полное условие с деталями вариантов доступно в исходном репозитории._

## Основные файлы

- [lab-client/src/main/java/client/Client.java](./lab-client/src/main/java/client/Client.java)
- [lab-client/src/main/java/client/ConsoleClient.java](./lab-client/src/main/java/client/ConsoleClient.java)
- [lab-client/src/main/java/client/GraphicClient.java](./lab-client/src/main/java/client/GraphicClient.java)
- [lab-client/src/main/java/client/GraphicClientNet.java](./lab-client/src/main/java/client/GraphicClientNet.java)
- [lab-server/src/main/java/server/Server.java](./lab-server/src/main/java/server/Server.java)
- [lab-server/src/main/java/server/ServerConfig.java](./lab-server/src/main/java/server/ServerConfig.java)
- [lab-server/src/main/java/server/ServerInstance.java](./lab-server/src/main/java/server/ServerInstance.java)
- [lab-client/src/main/java/client/locales/Locale_en_IN.java](./lab-client/src/main/java/client/locales/Locale_en_IN.java)
- [lab-client/src/main/java/client/locales/Locale_hu.java](./lab-client/src/main/java/client/locales/Locale_hu.java)
- [lab-client/src/main/java/client/locales/Locale_ro.java](./lab-client/src/main/java/client/locales/Locale_ro.java)
- [lab-client/src/main/java/client/locales/Locale_ru.java](./lab-client/src/main/java/client/locales/Locale_ru.java)
- Дополнительно: ещё **62** исходных файлов и ресурсов.

## Как запустить

Для проектов с `pom.xml` используйте установленную **Java + Maven**. В каталоге нужного модуля выполните `mvn compile` (при наличии необходимых зависимостей и сервисов).

