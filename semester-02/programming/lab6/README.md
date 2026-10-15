# Лабораторная №6 · Сервер

> **Программирование** · 2-й семестр · `ITMO / Нейротехнологии и программирование`

**Технологии:** Java · Maven

## Задача

Разделить программу из [лабораторной работы №5](https://github.com/CandyGoose/Programming_2_term_SE/tree/main/lab5) на клиентский и серверный модули. Серверный модуль должен осуществлять выполнение команд по управлению коллекцией. Клиентский модуль должен в интерактивном режиме считывать команды, передавать их для выполнения на сервер и выводить ре
**Необходимо выполнить следующие требования:**
- Операции обработки объектов коллекции должны быть реализованы с помощью Stream API с использованием лямбда-выражений.
- Объекты между клиентом и сервером должны передаваться в сериализованном виде.
- Объекты в коллекции, передаваемой клиенту, должны быть отсортированы по `имени`
- Клиент должен корректно обрабатывать временную недоступность сервера.
- Обмен данными между клиентом и сервером должен осуществляться по протоколу `TCP`
- Для обмена данными на сервере необходимо использовать `потоки ввода-вывода`
- Для обмена данными на клиенте необходимо использовать `сетевой канал`
- Сетевые каналы должны использоваться в неблокирующем режиме.
**Обязанности серверного приложения:**
- Работа с файлом, хранящим коллекцию.
- Управление коллекцией объектов.
- Назначение автоматически генерируемых полей объектов в коллекции.
- Ожидание подключений и запросов от клиента.
- Обработка полученных запросов (команд).
- Сохранение коллекции в файл при завершении работы приложения.
- Сохранение коллекции в файл при исполнении специальной команды, доступной только серверу (клиент такую команду отправить не может).
**Серверное приложение должно состоять из следующих модулей (реализованных в виде одного или нескольких классов):**
- Модуль приёма подключений.
- Модуль чтения запроса.

_Полное условие с деталями вариантов доступно в исходном репозитории._

## Основные файлы

- [lab-client/src/main/java/Client/Client.java](./lab-client/src/main/java/Client/Client.java)
- [lab-client/src/main/java/Client/ClientApp.java](./lab-client/src/main/java/Client/ClientApp.java)
- [lab-server/src/main/java/Server/ConsoleThread.java](./lab-server/src/main/java/Server/ConsoleThread.java)
- [lab-server/src/main/java/Server/Server.java](./lab-server/src/main/java/Server/Server.java)
- [lab-server/src/main/java/Server/ServerApp.java](./lab-server/src/main/java/Server/ServerApp.java)
- [lab-client/src/main/java/Client/CommandDispatcher/AvailableCommands.java](./lab-client/src/main/java/Client/CommandDispatcher/AvailableCommands.java)
- [lab-client/src/main/java/Client/CommandDispatcher/CommandListener.java](./lab-client/src/main/java/Client/CommandDispatcher/CommandListener.java)
- [lab-client/src/main/java/Client/CommandDispatcher/CommandToSend.java](./lab-client/src/main/java/Client/CommandDispatcher/CommandToSend.java)
- [lab-client/src/main/java/Client/CommandDispatcher/CommandValidators.java](./lab-client/src/main/java/Client/CommandDispatcher/CommandValidators.java)
- [lab-client/src/main/java/Client/util/ClientSocketChannelIO.java](./lab-client/src/main/java/Client/util/ClientSocketChannelIO.java)
- [lab-client/src/main/java/Client/util/RequestCreator.java](./lab-client/src/main/java/Client/util/RequestCreator.java)
- Дополнительно: ещё **41** исходных файлов и ресурсов.

## Как запустить

Для проектов с `pom.xml` используйте установленную **Java + Maven**. В каталоге нужного модуля выполните `mvn compile` (при наличии необходимых зависимостей и сервисов).

## Статус документации

Описание приведено по доступным материалам и структуре кода. Если оригинальный текст задания не сохранился, формулировка выше является кратким описанием реализации, а не официальным ТЗ.

## Источник

Материалы: [Programming_2_term_SE](https://github.com/CandyGoose/Programming_2_term_SE) · использование с разрешения исходного автора. Документация переработана для этого каталога.
