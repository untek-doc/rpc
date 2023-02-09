Аутентификация
===

Токен отправляется в виде заголовка `Authorization`.

Например:

```
Authorization: bearer nbVgQVbekPdO9E0AxEELaxj6FcwtJ06UM8pznMloPPd2~hySPUh6umsMWQtUkRGq
```

Если в ответ получаем [Аутентификация завершилась неудачно](../response/error/unauthrized.md), это означает,
что токен не актуальный.
В этом случае, получаем новый токен.
