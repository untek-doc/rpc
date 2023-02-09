Выборка полей
===

Список желаемых полей отправляется в виде body-параметра `fields`.

```json
{
  "jsonrpc": "2.0",
  "method": "my-contact.all",
  "params": {
    "body": {
      "fields": [
        "id",
        "title"
      ]
    }
  }
}
```

Будут выведены только указанные поля.
