Связи
===

Связи отправляются body-параметре `with`, в виде массива имен.

Обычно это вложенные записи.

## Пример для коллекции записей

```json
{
  "jsonrpc": "2.0",
  "method": "my-contact.all",
  "params": {
    "body": {
      "with": [
        "attribute"
      ]
    }
  }
}
```

В ответ получим записи с вложенностями:

```json
{
  "jsonrpc": "2.0",
  "result": {
    "body": [
      {
        "id": 1,
        "value": "support1@example.com",
        "attributeId": 1,
        "attribute": {
          "id": 1,
          "name": "email",
          "title": "Email"
        }
      },
      {
        "id": 2,
        "value": "+77771111111",
        "attributeId": 3,
        "attribute": {
          "id": 3,
          "name": "mobile",
          "title": "Мобильный номер"
        }
      },
      {
        "id": 19,
        "value": "+77771111211",
        "attributeId": 3,
        "attribute": {
          "id": 3,
          "name": "mobile",
          "title": "Мобильный номер"
        }
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

## Пример для одной записи

```json
{
  "jsonrpc": "2.0",
  "method": "my-contact.one-by-id",
  "params": {
    "body": {
      "id": 1,
      "with": [
        "attribute"
      ]
    }
  }
}
```

В ответ получим запись с вложенностью:

```json
{
  "jsonrpc": "2.0",
  "result": {
    "body": {
      "id": 1,
      "value": "support1@example.com",
      "attributeId": 1,
      "attribute": {
        "id": 1,
        "name": "email",
        "title": "Email"
      }
    }
  }
}
```
