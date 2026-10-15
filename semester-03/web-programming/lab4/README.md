# Лабораторная №4 · Java EE + React

> **Веб-программирование** · 3-й семестр · `ITMO / Нейротехнологии и программирование`

**Технологии:** Java · JavaScript · HTML · CSS · Maven

## Задача

Переписать приложение из [предыдущей лабораторной работы](https://github.com/CandyGoose/Web_programming_SE/tree/main/lab3) с использованием следующих технологий:
- Уровень back-end должен быть основан на `Java EE (необходимо использовать EJB)`.
- Уровень front-end должен быть построен на `React + Redux (необходимо использовать ES6 и JSX)` с использованием `набора компонентов PrimeReact`
- Взаимодействие между уровнями back-end и front-end должно быть организовано посредством REST API.
Приложение по-прежнему должно включать в себя 2 страницы - стартовую и основную страницу приложения. Обе страницы приложения должны быть адаптированы для отображения в 3 режимах:
- "Десктопный" - для устройств, ширина экрана которых равна или превышает `1101` пикселей.
- "Планшетный" - для устройств, ширина экрана которых равна или превышает `810`, но меньше `1101` пикселей.
- "Мобильный"- для устройств, ширина экрана которых меньше `810` пикселей.
__Стартовая страница должна содержать следующие элементы:__
- "Шапку", содержащую ФИО студента, номер группы и номер варианта.
- Форму для ввода логина и пароля. Информация о зарегистрированных в системе пользователях должна храниться в отдельной таблице БД (пароль должен храниться в виде хэш-суммы). Доступ неавторизованных пользователей к основной странице приложения должен быть запрещён.
__Основная страница приложения должна содержать следующие элементы:__

_Полное условие с деталями вариантов доступно в исходном репозитории._

## Основные файлы

- [frontend/public/index.html](./frontend/public/index.html)
- [frontend/src/App.js](./frontend/src/App.js)
- [frontend/src/index.js](./frontend/src/index.js)
- [frontend/src/app/store.js](./frontend/src/app/store.js)
- [backend/src/main/java/MainApplication.java](./backend/src/main/java/MainApplication.java)
- [frontend/src/app/api/apiSlice.js](./frontend/src/app/api/apiSlice.js)
- [frontend/src/components/auth/authApiSlice.js](./frontend/src/components/auth/authApiSlice.js)
- [frontend/src/components/auth/authSlice.js](./frontend/src/components/auth/authSlice.js)
- [frontend/src/components/auth/LoginPage.js](./frontend/src/components/auth/LoginPage.js)
- [frontend/src/components/auth/RegistrationPage.js](./frontend/src/components/auth/RegistrationPage.js)
- [frontend/src/components/auth/RequireAuth.js](./frontend/src/components/auth/RequireAuth.js)
- Дополнительно: ещё **29** исходных файлов и ресурсов.

## Как запустить

Для проектов с `pom.xml` используйте установленную **Java + Maven**. В каталоге нужного модуля выполните `mvn compile` (при наличии необходимых зависимостей и сервисов).

