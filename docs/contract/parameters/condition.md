Фильтрация
===

Условия фильтрации отправляются в виде body-параметров в ключе `filter`.

Можно задать фильтрацию по значению атрибута:

```json
{
  "jsonrpc": "2.0",
  "method": "my-contact.all",
  "params": {
    "body": {
      "filter": {
        "attributeId": 1
      }
    }
  }
}
```

Или сразу по нескольким атрибутам:

```json
{
  "jsonrpc": "2.0",
  "method": "my-contact.all",
  "params": {
    "body": {
      "filter": {
        "attributeId": 1,
        "statusId": 200
      }
    }
  }
}
```

При этом, условия буду склеены оператором `AND`.
