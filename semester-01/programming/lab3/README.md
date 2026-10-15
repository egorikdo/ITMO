# Лабораторная №3 · Объектная модель приложения по тексту

> **Программирование** · 1-й семестр · `ITMO / Нейротехнологии и программирование`

**Технологии:** Java

## Задача

2. Программа должна содержать как минимум два интерфейса и один абстрактный класс (номенклатура должна быть согласована с преподавателем).
3. В разработанных классах должны быть переопределены методы `equals()`, `toString()` и `hashCode()`.
4. Программа должна содержать как минимум один перечисляемый тип (enum).
1. Доработать объектную модель приложения.
2. Перерисовать диаграмму классов в соответствии с внесёнными в модель изменениями.
3. Согласовать с преподавателем изменения, внесённые в модель.
4. Модифицировать программу в соответствии с внесёнными в модель изменениями.
2. Диаграмма классов объектной модели.

## Основные файлы

- [src/Story.java](./src/Story.java)
- [src/abilities/IHelp.java](./src/abilities/IHelp.java)
- [src/abilities/IInstruct.java](./src/abilities/IInstruct.java)
- [src/abilities/IPhoneActions.java](./src/abilities/IPhoneActions.java)
- [src/abilities/IWalkAway.java](./src/abilities/IWalkAway.java)
- [src/abilities/IWalkToRoom.java](./src/abilities/IWalkToRoom.java)
- [src/enums/Gender.java](./src/enums/Gender.java)
- [src/enums/HearType.java](./src/enums/HearType.java)
- [src/enums/HelpType.java](./src/enums/HelpType.java)
- [src/enums/HouseRooms.java](./src/enums/HouseRooms.java)
- [src/enums/Instructions.java](./src/enums/Instructions.java)
- Дополнительно: ещё **10** исходных файлов и ресурсов.

## Как запустить

Используйте **JDK** и IDE (IntelliJ IDEA) либо `javac`/`java`. Для многомодульных проектов потребуется настройка classpath и дополнительных зависимостей.

## Статус документации

Описание приведено по доступным материалам и структуре кода. Если оригинальный текст задания не сохранился, формулировка выше является кратким описанием реализации, а не официальным ТЗ.

## Источник

Материалы: [Programming_1_term_SE](https://github.com/CandyGoose/Programming_1_term_SE) · использование с разрешения исходного автора. Документация переработана для этого каталога.
