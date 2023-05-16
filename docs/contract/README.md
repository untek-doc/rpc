# Контракт JSON-RPC API

## Начало

* [Введение](intro.md)
* [Meta-данные](meta.md)
* [RPC-методы](method.md)

## CRUD

* [Общая информация](crud/main.md)
* [Получение коллекции записей](crud/all.md)
* [Получение одной записи](crud/one.md)
* [Создание новой записи](crud/create.md)
* [Редактирование записи](crud/update.md)
* [Удаление записи](crud/delete.md)

## Локальные параметры

 * [Связи](parameters/relation.md)
 * [Выборка полей](parameters/fields.md)
 * [Пагинация](parameters/pagination.md)
 * [Сортировка](parameters/sort.md)
 * [Фильтрация](parameters/condition.md)

## Глобальные параметры

 * [Аутентификация](parameters/authenticate.md)
 * [Часовой пояс](parameters/time-zone.md)
 * [Мультиязычность](parameters/language.md)

## Форматы ответов от RPC

### Успешные ответы

* [Запрос обработан успешно и вернул пустое тело](response/success/empty.md)
* [Запрос обработан успешно и вернул данные](response/success/with-data.md)

### Ошибки

* [Метод объявлен устаревшим]()
* [Неверный запрос](response/error/bad-request.md)
* [Запись уже существует](response/error/exist.md)
* [Доступ запрещен](response/error/forbidden.md)
* [Внутренняя ошибка сервера](response/error/internal-error.md)
* [Запрошенный ресурс не существует](response/error/not-found.md)
* [Аутентификация завершилась неудачно](response/error/unauthrized.md)
* [Ошибка валидации данных](response/error/unpocessable.md)

## Разное

* [Формат времени](time-format.md)
* [Версионность](version.md)
