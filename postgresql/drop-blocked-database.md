#postgresql
#database
#drop
#blocked

```log
postgres=# DROP DATABASE <database-name>;
ERROR:  database "<database-name>" is being accessed by other users
DETAIL:  There are 4 other sessions using the database.
```

> prevent thhe future connections
```psql
REVOKE CONNECT ON DATABASE <database-name> FROM public;
```

> terminate connections
```psql
SELECT pid, pg_terminate_backend(pid)
FROM pg_stat_activity
WHERE datname = current_database() AND pid <> pg_backend_pid();
```

