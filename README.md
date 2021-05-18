## PostgreSQL

#### Create Role

CREATE ROLE professores NOCREATEDB NOCREATEROLE INHERIT NOLOGIN NOBYPASSRLS CONNECTION LIMIT 10;



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

![image-20210518160536071](C:\Users\edson.dasilva\AppData\Roaming\Typora\typora-user-images\image-20210518160536071.png)









