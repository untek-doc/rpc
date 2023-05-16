# Запрос обработан успешно и вернул данные

Все сработало именно так, как и ожидалось.

Данные возвращаются в теле ответа.

Может быть возвращена одна запись:

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

или коллекция записей:

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

или любая другая структура данных (включая `null`):

```json
{
  "jsonrpc": "2.0",
  "result": {
    "body": null
  }
}
```
