# Icosa Gallery Docker

Docker environment for the Icosa Gallery

## Config files

Copy the following files:

- `cp example.env .env`
- `cp config.example.json config.json`
- `cp gcp-service-account.example.json gcp-service-account.json`

Or create and fill them in manually. 

When running in docker, the api service needs its host specified as `db` instead of `localhost` where `db` is the postgres service name. This is currently set in the `dblocation` key inside `config.json`.


## First run

TODO: When running  `docker compose up -d` for the first time, the api service may start before postgres is fully available and fail to start. Subsequent runs should work as expected.
