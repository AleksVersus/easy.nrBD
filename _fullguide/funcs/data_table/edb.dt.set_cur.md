#### edb.dt.set_cur

Устанавливает указанную таблицу данных текущей.

Аргументы:

* `$args[0]` — идентификатор таблицы данных.

Идентификатор текущей таблицы данных записывается в `$EASY_DATABASE['last_data_table']`, а идентификатор указанной таблицы данных записывается в `$EASY_DATABASE['current_data_table']`.

Пример:

```qsp
@edb.dt.set_cur('object')
```
