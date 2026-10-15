# Лабораторная №3 · Симуляция архитектуры компьютера

> **Архитектура компьютера** · 4-й семестр · `ITMO / Нейротехнологии и программирование`

**Технологии:** Python · Assembler

## Задача

Реализовать вычислительный эксперимент по теме «Симуляция архитектуры компьютера» с помощью Python. Детальные требования в переданном архиве не сохранились.

## Основные файлы

- [golden_asm_test.py](./golden_asm_test.py)
- [simulation.py](./simulation.py)
- [translator.py](./translator.py)
- [machine/cpu.py](./machine/cpu.py)
- [machine/decoder.py](./machine/decoder.py)
- [machine/io_ports.py](./machine/io_ports.py)
- [machine/isa.py](./machine/isa.py)
- [machine/logger.py](./machine/logger.py)
- [machine/machine_signals.py](./machine/machine_signals.py)

## Как запустить

Понадобятся компилятор **GCC/Clang**, `make` и инструменты, указанные в коде. Для xv6 также нужен **QEMU**. Команды сборки зависят от конкретной версии проекта.

## Статус документации

Описание приведено по доступным материалам и структуре кода. Если оригинальный текст задания не сохранился, формулировка выше является кратким описанием реализации, а не официальным ТЗ.

## Источник

Материалы: [Computer_architecture](https://github.com/CandyGoose/Computer_architecture) · использование с разрешения исходного автора. Документация переработана для этого каталога.
