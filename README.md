freecodecamp Celestial Bodies Database project (disclaimer: database is NOT factual)
### To save/dump the database

In bash:
```bash
pg_dump -U postgres universe > universe.sql
```

### To restore the dump

1. Start PostgreSQL

2. In bash:
```bash
psql --username=freecodecamp --dbname=postgres
```

3. In psql:
```sql
CREATE DATABASE universe;
\q
```

4. In bash:
```bash
psql -U postgres -d universe -f universe.sql
```
