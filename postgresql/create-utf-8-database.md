#postgresql
#utf8 #utf-8
#encoding
#with-owner

```sql
CREATE DATABASE <database-name>
    WITH OWNER '<owner>'
    ENCODING 'UTF8'
    LC_COLLATE = 'en_US.UTF-8'
    LC_CTYPE = 'en_US.UTF-8'
    TEMPLATE template0;
```

> TEMPLATE template0 is required if the default encoding is not UTF-8
```log
ERROR:  new encoding (UTF8) is incompatible with the encoding of the template database (SQL_ASCII)
HINT:  Use the same encoding as in the template database, or use template0 as template.
```
