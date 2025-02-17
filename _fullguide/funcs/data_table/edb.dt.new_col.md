#### edb.dt.new_col

Создаёт колонку в таблице данных.

Аргументы:

* `$args[0]` — идентификатор колонки. Обязательный аргумент.
* `$args[1]` — тип колонки. По умолчанию, тип '`str`'.
* `$args[2]` — идентификатор таблицы данных. Если не указан, используется текущий.

Примеры вызова:

```qsp
@edb.dt.new_col('body', 'dict', 'objects')
@edb.dt.new_col('place', 'str', 'objects')
@edb.dt.new_col('include')
@edb.dt.new_col('count', 'num')
```

При создании колонки в таблице данных инициализируется массив с именем, состоящим из идентификатора таблицы данных и идентификатора колонки данных, поэтому к идентификатору колонки применяются те же требования, что и к названиям массивов в QSP. Например, если идентификатор таблицы данных `objects`, а идентификатор колонки `body`, будет инициализирован массив `$objects_body`.

При создании колонки, [её тип](_fullguide/data_types.md) записывается в массив таблицы данных в ячейку с текстовым индексом `column.COLUMN_ID.type`, где `COLUMN_ID` — идентификатор колонки.
