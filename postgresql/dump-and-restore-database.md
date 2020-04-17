#postgresql
#database
#dump
#restore
#remote

## dump
```bash
pg_dump <database-name> > <backup-file-name>
```

### remote
```bash
pg_dump -U <user-name> -p <remote-port> <database-name> > <backup-file-name>
```

## restore
```bash
#createdb -T template0 <restored-database-name>
psql <restored-database-name> < <backup-file>
```
