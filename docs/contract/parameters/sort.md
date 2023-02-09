Сортировка
===

Сортировка отправляется в виде body-параметра `order`.

Возможные направления сортировки:

* `asc` - по возрастанию
* `desc` - по убыванию

Можно сортировать как по одному полю, так и нескольким полям сразу.

```json
{
  "jsonrpc": "2.0",
  "method": "my-contact.all",
  "params": {
    "body": {
      "order": {
        "title": "asc",
        "id": "desc"
      }
    }
  }
}
```