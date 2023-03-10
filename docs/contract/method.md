# RPC-методы

RPC-методы используются для идентификации обработчика запроса.

Допускается использовать разделитель токчу `.` 
для отделения контекста от выполняемой операции.

## Соглашения об именовании

* Названия всегда давайте в **единственном числе**.
* Названия всегда пишите **строчными буквами**.
* Названия делайте как можно **проще**.
* **Используйте** в именах только буквы, цифры и тире.
* **Используйте** **kebab-case** стиль именования.
* **Убедитесь** в том, что имя уникально.
* **Начинайте** имена с буквы и **не заканчивайте** их символом тире.
* **Избегайте** сокращений. Если их всё же нужно использовать, убедитесь в том, что они общепонятны.
* **Избегайте** нескольких подряд идущих символов тире.

## Примеры

* `authentication.get-token-by-password` - получить токен аутентификации, предоставив логин/пароль
* `my-contact.all` - получить список моих контактов
* `my-contact.create` - добавить мой новый контакт
* `my-contact.update` - редактировать мой контакт
* `my-contact.delete` - удалить мой контакт
