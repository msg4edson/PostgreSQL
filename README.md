# PostgreSQL


## Administrar usuário no banco de dados

#### Create Role

CREATE ROLE professores NOCREATEDB NOCREATEROLE INHERIT NOLOGIN NOBYPASSRLS CONNECTION LIMIT 10;

CREATE ROLE daniel LOGIN PASSWORD '123';

CREATE ROLE daniel LOGIN PASSWORD '123' IN ROLE professores;

CREATE ROLE daniel INHERIT LOGIN PASSWORD '123' IN ROLE professores;



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

#### Grant

GRANT ALL ON TABLE teste TO professores;


#### Revoke Role

REVOKE professores FROM daniel;


## Objetos e comandos do banco de dados

