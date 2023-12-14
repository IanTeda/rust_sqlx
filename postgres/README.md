# Postgres and pgAdmin

Spin up an Postgres database with pgAdmin database administration

## Initialisation

Copy the `env.sample` to `.env` and make any changes you need.

```sh
cp env.sample .env
```

## Start

Change directory into the postgres directory and run the command

```sh
docker-compose up -d
```

Check that Postgres is up and running

```sh
docker ps
```

Check the Postgres container log

```sh
docker logs -f -t rust_sqlx_postgres 
```

Check the pgAdmin container log 

```sh
docker logs -f -t rust_sqlx_pgadmin
```

## Stop 

Change directory into postgres directory and run the command

```sh
docker-compose down
```

## Access 

By default pgAdmin can be reached at [http://127.0.0.1:15433](http://127.0.0.1:15433)


#### References

- [Docker-Compose with PostgreSQL ready to use](https://github.com/felipewom/docker-compose-postgres)
