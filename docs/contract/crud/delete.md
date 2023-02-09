# Удаление записи

Удаление контакта с id равным 123:

Запрос:

```json
{
  "jsonrpc": "2.0",
  "method": "my-contact.delete",
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
        "body": null
    }
}
```

Возможные варианты ответов:

* [Запрос обработан успешно и вернул пустое тело](../response/success/empty.md)
* [Запрошенный ресурс не существует](../response/error/not-found.md)
* [Внутренняя ошибка сервера](../response/error/internal-error.md)
