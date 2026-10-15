# Лабораторная №2 · JSP + Servlets

> **Веб-программирование** · 3-й семестр · `ITMO / Нейротехнологии и программирование`

**Технологии:** Java · JavaScript · CSS · Maven

## Задача

__Изменения данных__
- изменение X: Button {'-5', '-4', '-3', '-2', '-1', '0', '1', '2', '3'}
- изменение Y: Text (-3 … 5)
- Изменение R: Radio {'1', '2', '3', '4', '5'}
- метод HTTP: GET
- список результатов сохранять в Bean-компоненте
Разработать веб-приложение на базе сервлетов и JSP, определяющее попадание точки на координатной плоскости в заданную область.
Приложение должно быть реализовано в соответствии с [шаблоном MVC](https://en.wikipedia.org/wiki/Model–view–controller) и состоять из следующих элементов:
- __ControllerServlet__, определяющий тип запроса, и, в зависимости от того, содержит ли запрос информацию о координатах точки и радиусе, делегирующий его обработку одному из перечисленных ниже компонентов. Все запросы внутри приложения должны передаваться этому сервлету (по методу GET или POST в зависимости от варианта задания), остальные сервлеты
- __AreaCheckServlet__, осуществляющий проверку попадания точки в область на координатной плоскости и формирующий HTML-страницу с результатами проверки. Должен обрабатывать все запросы, содержащие сведения о координатах точки и радиусе области.
- __Страница JSP__, формирующая HTML-страницу с веб-формой. Должна обрабатывать все запросы, не содержащие сведений о координатах точки и радиусе области.
__Разработанная страница JSP должна содержать:__
1. "Шапку", содержащую ФИО студента, номер группы и номер варианта.
2. Форму, отправляющую данные на сервер.
3. Набор полей для задания координат точки и радиуса области в соответствии с вариантом задания.
4. Сценарий на языке JavaScript, осуществляющий валидацию значений, вводимых пользователем в поля формы.

_Полное условие с деталями вариантов доступно в исходном репозитории._

## Основные файлы

- [src/main/java/data/Coordinates.java](./src/main/java/data/Coordinates.java)
- [src/main/java/data/Result.java](./src/main/java/data/Result.java)
- [src/main/java/data/ResultContainer.java](./src/main/java/data/ResultContainer.java)
- [src/main/java/servlets/AreaCheckServlet.java](./src/main/java/servlets/AreaCheckServlet.java)
- [src/main/java/servlets/ControllerServlet.java](./src/main/java/servlets/ControllerServlet.java)
- [src/main/webapp/js/check.js](./src/main/webapp/js/check.js)
- [src/main/webapp/js/form.js](./src/main/webapp/js/form.js)
- [src/main/webapp/js/script.js](./src/main/webapp/js/script.js)
- [src/main/webapp/js/utils.js](./src/main/webapp/js/utils.js)
- [src/main/java/servlets/filters/UrlFilter.java](./src/main/java/servlets/filters/UrlFilter.java)
- [src/main/java/servlets/listeners/DataLoader.java](./src/main/java/servlets/listeners/DataLoader.java)

## Как запустить

Для проектов с `pom.xml` используйте установленную **Java + Maven**. В каталоге нужного модуля выполните `mvn compile` (при наличии необходимых зависимостей и сервисов).

