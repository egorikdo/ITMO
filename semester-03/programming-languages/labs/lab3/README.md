# Лабораторная №3 · Поворот картинки

> **Языки программирования** · 3-й семестр · `ITMO / Нейротехнологии и программирование`

**Технологии:** C

## Задача

Лабораторная работа: Поворот картинки
- Необходимо реализовать поворот изображения в формате BMP на 90 градусов против
часовой стрелки. Формат использования такой:
- Архитектура приложения описана в предыдущем разделе.
- Код размещается в директории `solution/src`, заголовочные файлы ищутся в `solution/include`.

## Основные файлы

- [solution/src/bmp_io.c](./solution/src/bmp_io.c)
- [solution/src/image.c](./solution/src/image.c)
- [solution/src/main.c](./solution/src/main.c)
- [solution/src/transformations.c](./solution/src/transformations.c)
- [tester/src/bmp.c](./tester/src/bmp.c)
- [tester/src/file_cmp.c](./tester/src/file_cmp.c)
- [tester/src/main.c](./tester/src/main.c)
- [tester/src/util.c](./tester/src/util.c)

## Как запустить

Понадобятся компилятор **GCC/Clang**, `make` и инструменты, указанные в коде. Для xv6 также нужен **QEMU**. Команды сборки зависят от конкретной версии проекта.

