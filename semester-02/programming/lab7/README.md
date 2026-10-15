# Лабораторная №7 · БД

> **Программирование** · 2-й семестр · `ITMO / Нейротехнологии и программирование`

**Технологии:** Java · Maven

## Задача

Доработать программу из [лабораторной работы №6](https://github.com/CandyGoose/Programming_2_term_SE/tree/main/lab6) следующим образом:
1. Организовать хранение коллекции в реляционной СУБД (PostgresQL). Убрать хранение коллекции в файле.
2. Для генерации поля id использовать средства базы данных (sequence).
3. Обновлять состояние коллекции в памяти только при успешном добавлении объекта в БД
4. Все команды получения данных должны работать с коллекцией в памяти, а не в БД
5. Организовать возможность регистрации и авторизации пользователей. У пользователя есть возможность указать пароль.
6. Пароли при хранении хэшировать алгоритмом `SHA-1`
7. Запретить выполнение команд не авторизованным пользователям.
8. При хранении объектов сохранять информацию о пользователе, который создал этот объект.
9. Пользователи должны иметь возможность просмотра всех объектов коллекции, но модифицировать могут только принадлежащие им.
10. Для идентификации пользователя отправлять логин и пароль с каждым запросом.
Необходимо реализовать многопоточную обработку запросов.
1. Для многопоточного чтения запросов использовать `Fixed thread pool`
2. Для многопотчной обработки полученного запроса использовать `Fixed thread pool`
3. Для многопоточной отправки ответа использовать `Fixed thread pool`
4. Для синхронизации доступа к коллекции использовать `потокобезопасные аналоги коллекции из java.util.concurrent`
**Порядок выполнения работы:**
1. В качестве базы данных использовать PostgreSQL.
2. Для подключения к БД на кафедральном сервере использовать хост _pg_, имя базы данных - _studs_, имя пользователя/пароль совпадают с таковыми для подключения к серверу.
**Дополнительные условия:**

_Полное условие с деталями вариантов доступно в исходном репозитории._

## Основные файлы

- [lab-client/src/main/java/Client/App.java](./lab-client/src/main/java/Client/App.java)
- [lab-client/src/main/java/Client/Client.java](./lab-client/src/main/java/Client/Client.java)
- [lab-server/src/main/java/Server/App.java](./lab-server/src/main/java/Server/App.java)
- [lab-server/src/main/java/Server/AppConfig.java](./lab-server/src/main/java/Server/AppConfig.java)
- [lab-server/src/main/java/Server/Server.java](./lab-server/src/main/java/Server/Server.java)
- [lab-server/src/main/java/Server/ServerConfig.java](./lab-server/src/main/java/Server/ServerConfig.java)
- [lab-client/src/main/java/Client/CommandDispatcher/AvailableCommands.java](./lab-client/src/main/java/Client/CommandDispatcher/AvailableCommands.java)
- [lab-client/src/main/java/Client/CommandDispatcher/CommandListener.java](./lab-client/src/main/java/Client/CommandDispatcher/CommandListener.java)
- [lab-client/src/main/java/Client/CommandDispatcher/CommandToSend.java](./lab-client/src/main/java/Client/CommandDispatcher/CommandToSend.java)
- [lab-client/src/main/java/Client/CommandDispatcher/CommandValidators.java](./lab-client/src/main/java/Client/CommandDispatcher/CommandValidators.java)
- [lab-client/src/main/java/Client/NetworkManager/AuthorizationModule.java](./lab-client/src/main/java/Client/NetworkManager/AuthorizationModule.java)
- Дополнительно: ещё **51** исходных файлов и ресурсов.

## Как запустить

Для проектов с `pom.xml` используйте установленную **Java + Maven**. В каталоге нужного модуля выполните `mvn compile` (при наличии необходимых зависимостей и сервисов).

## Статус документации

Описание приведено по доступным материалам и структуре кода. Если оригинальный текст задания не сохранился, формулировка выше является кратким описанием реализации, а не официальным ТЗ.

## Источник

Материалы: [Programming_2_term_SE](https://github.com/CandyGoose/Programming_2_term_SE) · использование с разрешения исходного автора. Документация переработана для этого каталога.
