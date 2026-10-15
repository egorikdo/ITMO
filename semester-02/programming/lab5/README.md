# Лабораторная №5 · Консольное приложение

> **Программирование** · 2-й семестр · `ITMO / Нейротехнологии и программирование`

**Технологии:** Java · Maven

## Задача

Реализовать консольное приложение, которое реализует управление коллекцией объектов в интерактивном режиме. В коллекции необходимо хранить объекты класса **Organization**, описание которого приведено ниже.
**Разработанная программа должна удовлетворять следующим требованиям:**
- Класс, коллекцией экземпляров которого управляет программа, должен реализовывать сортировку по умолчанию.
- Все требования к полям класса (указанные в виде комментариев) должны быть выполнены.
- Для хранения необходимо использовать коллекцию типа `java.util.LinkedList`
- При запуске приложения коллекция должна автоматически заполняться значениями из файла.
- Имя файла должно передаваться программе с помощью: `переменная окружения`.
- Данные должны храниться в файле в формате `xml`
- Чтение данных из файла необходимо реализовать с помощью класса `java.util.Scanner`
- Запись данных в файл необходимо реализовать с помощью класса `java.io.BufferedOutputStream`
- Все классы в программе должны быть задокументированы в формате javadoc.
- Программа должна корректно работать с неправильными данными (ошибки пользовательского ввода, отсутсвие прав доступа к файлу и т.п.).
**В интерактивном режиме программа должна поддерживать выполнение следующих команд:**
- *help* : вывести справку по доступным командам
- *info* : вывести в стандартный поток вывода информацию о коллекции (тип, дата инициализации, количество элементов и т.д.)
- *show* : вывести в стандартный поток вывода все элементы коллекции в строковом представлении
- *add {element}* : добавить новый элемент в коллекцию
- *update id {element}* : обновить значение элемента коллекции, id которого равен заданному

_Полное условие с деталями вариантов доступно в исходном репозитории._

## Основные файлы

- [src/main/java/App.java](./src/main/java/App.java)
- [src/main/java/commands/AbstractCommand.java](./src/main/java/commands/AbstractCommand.java)
- [src/main/java/commands/AddCommand.java](./src/main/java/commands/AddCommand.java)
- [src/main/java/commands/ClearCommand.java](./src/main/java/commands/ClearCommand.java)
- [src/main/java/commands/ExecuteScriptCommand.java](./src/main/java/commands/ExecuteScriptCommand.java)
- [src/main/java/commands/ExitCommand.java](./src/main/java/commands/ExitCommand.java)
- [src/main/java/commands/HelpCommand.java](./src/main/java/commands/HelpCommand.java)
- [src/main/java/commands/HistoryCommand.java](./src/main/java/commands/HistoryCommand.java)
- [src/main/java/commands/ICommand.java](./src/main/java/commands/ICommand.java)
- [src/main/java/commands/InfoCommand.java](./src/main/java/commands/InfoCommand.java)
- [src/main/java/commands/PrintDescendingCommand.java](./src/main/java/commands/PrintDescendingCommand.java)
- Дополнительно: ещё **25** исходных файлов и ресурсов.

## Как запустить

Для проектов с `pom.xml` используйте установленную **Java + Maven**. В каталоге нужного модуля выполните `mvn compile` (при наличии необходимых зависимостей и сервисов).

