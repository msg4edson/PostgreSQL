## PostgreSQL

#### Create Role

CREATE ROLE professores NOCREATEDB NOCREATEROLE INHERIT NOLOGIN NOBYPASSRLS CONNECTION LIMIT 10;



Open via CMD:

cd C:\Program Files\PostgreSQL\11\bin

psql -U postgres -h localhost



postgres=# \du
To List of roles

SELECT * FROM gp_roles;



