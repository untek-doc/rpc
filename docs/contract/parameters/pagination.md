Пагинация
===

Инфо о пагинации отправляется в виде body-параметров `page`, `perPage`.

## Параметры

`page` - Текущая страница

`perPage` - Количество записей странице

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

## Получаемые meta-данные

* page - Текущая страница
* perPage - Количество записей на страницу
* totalCount - Количество всех записей

```json
{
  "jsonrpc": "2.0",
  "result": {
    "meta": {
      "perPage": 20,
      "totalCount": 3
    }
  }
}
```
