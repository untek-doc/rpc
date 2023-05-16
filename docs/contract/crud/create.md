# Создание новой записи

В теле запроса отправляем значения атрибутов записи:

Запрос:

```json
{
  "jsonrpc": "2.0",
  "method": "my-contact.create",
  "params": {
    "body": {
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
      "id": 1,
      "value": "+77771111211",
      "attributeId": 3
    }
  }
}
```

Возможные варианты ответов:

* [Запрос обработан успешно и вернул данные](../response/success/with-data.md)
* [Запись уже существует](../response/error/exist.md)
* [Ошибка валидации данных](../response/error/unpocessable.md)
* [Внутренняя ошибка сервера](../response/error/internal-error.md)
