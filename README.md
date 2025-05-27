# Postgres Server in Docker

Run Postgres Server in Docker for local development.

### Configs

Create a config file `configs/config.env` by copying from `configs/config.env.example`, and update environment values.

```bash
# create new config file
cp configs/config.env.example configs/config.env

# update config values
POSTGRES_IMAGE_TAG=14
POSTGRES_PORT=5432
POSTGRES_DB=postgresdb
```

### Secrets

Create three secret files inside `secrets/` directory, and add values to them.

- postgres-user.txt
- postgres-password.txt

### Run Commands

```bash
# start mysql server
task dc-up

# stop mysql server
task dc-stop

# remove mysql server
task dc-down

# show container logs
task dc-logs
```
