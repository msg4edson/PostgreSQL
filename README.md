<<<<<<< HEAD
=======
# PostgreSQL


## Administrar usuário no banco de dados

#### Create Role

CREATE ROLE professores NOCREATEDB NOCREATEROLE INHERIT NOLOGIN NOBYPASSRLS CONNECTION LIMIT 10;

CREATE ROLE daniel LOGIN PASSWORD '123';

CREATE ROLE daniel LOGIN PASSWORD '123' IN ROLE professores;



Open via CMD:

cd C:\Program Files\PostgreSQL\11\bin

psql -U postgres -h localhost



postgres=# \du
To List of roles

SELECT * FROM gp_roles;

#### Alter Role

ALTER ROLE professores PASSWORD '123';

Open via CMD:

\q

#### Drop Role

DROP ROLE daniel;










>>>>>>> 35c0d03132b396e3fb901aa71f101ffca44bba96

