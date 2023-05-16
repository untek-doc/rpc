# Получение коллекции записей

Получение коллекции моих контактов постранично.

Запрос:

```json
{
  "jsonrpc": "2.0",
  "method": "my-contact.all",
  "params": {
    "body": {
      "page": 1,
      "perPage": 20
    }
  }
}
```

Ответ:

```json
{
  "jsonrpc": "2.0",
  "result": {
    "body": [
      {
        "id": 1,
        "value": "support1@example.com",
        "attributeId": 1
      },
      {
        "id": 2,
        "value": "+77771111111",
        "attributeId": 3
      },
      {
        "id": 19,
        "value": "+77771111211",
        "attributeId": 3
      }
    ],
    "meta": {
      "perPage": 20,
      "totalCount": 3,
      "page": 1
    }
  }
}
```

Можем использовать параметры в `body`:

* [Связи](../parameters/relation.md)
* [Выборка полей](../parameters/fields.md)
* [Пагинация](../parameters/pagination.md)
* [Сортировка](../parameters/sort.md)
* [Фильтрация](../parameters/condition.md)

Возможные варианты ответов:

* [Запрос обработан успешно и вернул данные](../response/success/with-data.md)
* [Неверный запрос](../response/error/bad-request.md)
* [Внутренняя ошибка сервера](../response/error/internal-error.md)
