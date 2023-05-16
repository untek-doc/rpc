# Редактирование записи

Изменение информации по контакту с id равным 123.

В теле запроса отправляем ID и новые значения атрибутов записи:

Запрос:

```json
{
  "jsonrpc": "2.0",
  "method": "my-contact.update",
  "params": {
    "body": {
      "id": 123,
      "value": "+77771111211",
      "attributeId": 3
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
      "id": 123,
      "value": "+77771111211",
      "attributeId": 3
    }
  }
}
```

Можно изменять атрубуты по отдельности:

```json
{
  "jsonrpc": "2.0",
  "method": "my-contact.update",
  "params": {
    "body": {
      "id": 123,
      "value": "+77771111211"
    }
  }
}
```

Возможные варианты ответов:

* [Запрос обработан успешно и вернул данные](../response/success/with-data.md)
* [Ошибка валидации данных](../response/error/unpocessable.md)
* [Внутренняя ошибка сервера](../response/error/internal-error.md)
