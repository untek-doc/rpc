# Получение одной записи

Получение информации по конкретному контакту с id равным 123:

Запрос:

```json
{
  "jsonrpc": "2.0",
  "method": "my-contact.one-by-id",
  "params": {
    "body": {
      "id": 123
    }
  }
}
```

Ответ:

```json
{
  "jsonrpc": "2.0",
  "result": {
    "body": {
      "id": 1,
      "value": "support1@example.com",
      "attributeId": 1
    }
  }
}
```

Можем использовать параметры в `body`:

* [Связи](../parameters/relation.md)
* [Выборка полей](../parameters/fields.md)

Возможные варианты ответов:

* [Запрос обработан успешно и вернул данные](../response/success/with-data.md)
* [Запрошенный ресурс не существует](../response/error/not-found.md)
* [Внутренняя ошибка сервера](../response/error/internal-error.md)
