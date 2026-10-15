# Лабораторная №1 · Модификация и запуск xv6

> **Операционные системы** · 5-й семестр · `ITMO / Нейротехнологии и программирование`

**Технологии:** Python · C · Prolog

## Задача

1. [Первый запуск ОС Xv6: Linux](doc/setup/linux.md)
2. [Настройка IDE: VSCode](doc/dev/vscode.md)
3. [Подготовка репозитория](doc/setup/repo.md)
1. [Задание 1. Введение в Xv6](doc/lab/1.md)
2. [Задание 2. Аллокатор](doc/lab/2.md)
3. [Задание 3. Copy-on-write fork](doc/lab/3.md)

## Основные файлы

- [kernel/bio.c](./kernel/bio.c)
- [kernel/buddy.c](./kernel/buddy.c)
- [kernel/console.c](./kernel/console.c)
- [kernel/exec.c](./kernel/exec.c)
- [kernel/file.c](./kernel/file.c)
- [kernel/fs.c](./kernel/fs.c)
- [kernel/kalloc.c](./kernel/kalloc.c)
- [kernel/list.c](./kernel/list.c)
- [kernel/log.c](./kernel/log.c)
- [kernel/main.c](./kernel/main.c)
- [kernel/pipe.c](./kernel/pipe.c)
- Дополнительно: ещё **51** исходных файлов и ресурсов.

## Как запустить

Понадобятся компилятор **GCC/Clang**, `make` и инструменты, указанные в коде. Для xv6 также нужен **QEMU**. Команды сборки зависят от конкретной версии проекта.

## Статус документации

Описание приведено по доступным материалам и структуре кода. Если оригинальный текст задания не сохранился, формулировка выше является кратким описанием реализации, а не официальным ТЗ.

## Источник

Материалы: [Operating_systems](https://github.com/CandyGoose/Operating_systems) · использование с разрешения исходного автора. Документация переработана для этого каталога.
