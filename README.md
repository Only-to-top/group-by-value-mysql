# group-by-value-mysql

```sql
SELECT * FROM reestr_object_mtx AS obj WHERE date_mtx = (SELECT MAX(date_mtx) FROM reestr_object_mtx WHERE `name_value` = obj.name_value AND id_object = $id) AND id_object = $id
```
