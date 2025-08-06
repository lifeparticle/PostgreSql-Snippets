# PostgreSql-Snippets

[How to Run PostgreSQL Using Docker](https://towardsdatascience.com/how-to-run-postgresql-using-docker-15bf87b452d4)

[How to Connect to a PostgreSQL Database With a Python Serverless Function](https://towardsdatascience.com/how-to-connect-to-a-postgresql-database-with-a-python-serverless-function-f5f3b244475)

[How to Connect to a Heroku Postgres Database With pgAdmin Using Docker](https://towardsdatascience.com/how-to-connect-to-a-heroku-postgres-database-with-pgadmin4-using-docker-6ac1e423ae66)

[How to Run PostgreSQL and pgAdmin Using Docker](https://towardsdatascience.com/how-to-run-postgresql-and-pgadmin-using-docker-3a6a8ae918b5)


```shell
brew services start postgresql
createuser -s postgres
brew services restart postgresql

brew unlink postgresql@13
brew link postgresql@12

brew info postgresql
```

```shell
psql -U mahbubzaman -d postgres
ALTER ROLE postgres WITH SUPERUSER;
```

```sql
brew services restart postgresql@14

psql postgres

# List of Roles 
\du

Role name  |                         Attributes                         | Member of 
-------------+------------------------------------------------------------+-----------
 mahbubzaman | Superuser | {}
 postgres    | Superuser | {}

# List of databases
\l

CREATE DATABASE DB_NAME;

# Select the db
\c DB_NAME

# Show tables
\dt


# Quit
\q

# Export CSV
COPY articles TO '/Users/xyz/Desktop/abc/article.csv' DELIMITER ',' CSV HEADER;

# Import CSV
COPY articles FROM '/Users/xyz/Desktop/abc/article.csv' DELIMITER ',' CSV HEADER;
```
