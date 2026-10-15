# Лабораторная №7

> **Программирование** · 2-й семестр · `ITMO / Нейротехнологии и программирование`

**Технологии:** Java · Maven

## Задача

Реализовать консольное приложение, которое реализует управление коллекцией объектов в интерактивном режиме. В коллекции необходимо хранить объекты класса `Person`, описание которого приведено ниже.
__Разработанная программа должна удовлетворять следующим требованиям:__
- Класс, коллекцией экземпляров которого управляет программа, должен реализовывать сортировку по умолчанию.
- Все требования к полям класса (указанные в виде комментариев) должны быть выполнены.
- Для хранения необходимо использовать коллекцию типа `java.util.LinkedList`
- При запуске приложения коллекция должна автоматически заполняться значениями из файла.
- Все классы в программе должны быть задокументированы в формате javadoc.
- Программа должна корректно работать с неправильными данными (ошибки пользовательского ввода, отсутсвие прав доступа к файлу и т.п.).
__В интерактивном режиме программа должна поддерживать выполнение следующих команд:__
- _help_ : вывести справку по доступным командам
- _info_ : вывести в стандартный поток вывода информацию о коллекции (тип, дата инициализации, количество элементов и т.д.)
- _show_ : вывести в стандартный поток вывода все элементы коллекции в строковом представлении
- _add {element}_ : добавить новый элемент в коллекцию
- _update id {element}_ : обновить значение элемента коллекции, id которого равен заданному
- _remove_by_id id_ : удалить элемент из коллекции по его id
- _clear_ : очистить коллекцию
- _save_ : сохранить коллекцию в файл
- _execute_script file_name_ : считать и исполнить скрипт из указанного файла. В скрипте содержатся команды в таком же виде, в котором их вводит пользователь в интерактивном режиме.

_Полное условие с деталями вариантов доступно в исходном репозитории._

## Основные файлы

- [lab-client/src/main/java/Client/App.java](./lab-client/src/main/java/Client/App.java)
- [lab-client/src/main/java/Client/Client.java](./lab-client/src/main/java/Client/Client.java)
- [lab-server/src/main/java/Server/App.java](./lab-server/src/main/java/Server/App.java)
- [lab-server/src/main/java/Server/Server.java](./lab-server/src/main/java/Server/Server.java)
- [lab-server/src/main/java/Server/ServerConfig.java](./lab-server/src/main/java/Server/ServerConfig.java)
- [lab-client/src/main/java/Client/CommandDispatcher/AvailableCommands.java](./lab-client/src/main/java/Client/CommandDispatcher/AvailableCommands.java)
- [lab-client/src/main/java/Client/CommandDispatcher/CommandListener.java](./lab-client/src/main/java/Client/CommandDispatcher/CommandListener.java)
- [lab-client/src/main/java/Client/CommandDispatcher/CommandToSend.java](./lab-client/src/main/java/Client/CommandDispatcher/CommandToSend.java)
- [lab-client/src/main/java/Client/CommandDispatcher/CommandValidators.java](./lab-client/src/main/java/Client/CommandDispatcher/CommandValidators.java)
- [lab-client/src/main/java/Client/NetworkManager/AuthorizationModule.java](./lab-client/src/main/java/Client/NetworkManager/AuthorizationModule.java)
- [lab-client/src/main/java/Client/NetworkManager/ClientSocketChannelIO.java](./lab-client/src/main/java/Client/NetworkManager/ClientSocketChannelIO.java)
- Дополнительно: ещё **52** исходных файлов и ресурсов.

## Как запустить

Для проектов с `pom.xml` используйте установленную **Java + Maven**. В каталоге нужного модуля выполните `mvn compile` (при наличии необходимых зависимостей и сервисов).

## Статус документации

Описание приведено по доступным материалам и структуре кода. Если оригинальный текст задания не сохранился, формулировка выше является кратким описанием реализации, а не официальным ТЗ.

## Источник

Материалы: [Programming_2_term_SE](https://github.com/CandyGoose/Programming_2_term_SE) · использование с разрешения исходного автора. Документация переработана для этого каталога.
