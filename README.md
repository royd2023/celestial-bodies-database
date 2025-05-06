To save/dump the database:
in bash: pg_dump -U postgres universe > universe.sql

To restore the dump:
- start postgresql
  
- in bash:
pg_dump -U postgres universe > universe.sql

- in psql:
CREATE DATABASE universe;\n
\q

- in bash:
psql -U postgres -d universe -f universe.sql
