# Docker Compose Guide

## The `services:` Block

The `services:` block defines the containers that make up the application. Each service represents a separate container with its own image and configuration.

In this project, there are two services:

* `database` - runs the MariaDB database.
* `app` - runs the Nextcloud application.

## How did the Nextcloud app container know how to find the database container?

The Nextcloud application finds the database through the `MYSQL_HOST` environment variable:

```yaml
- MYSQL_HOST=database
```

The value `database` is the name of the database service. Docker Compose allows the containers to communicate using their service names.

The Compose file uses environment variables to configure the database and Nextcloud application.

For example:

```yaml
- MYSQL_PASSWORD=cloudnova_pass
- MYSQL_DATABASE=nextcloud_db
- MYSQL_USER=nextcloud_user
```

These variables provide the database credentials and database name required by the application.


## Difference Between `docker run` and `docker-compose up -d`

## What is the difference between `docker run` and `docker-compose up -d`?

`docker run` starts a single Docker container with the settings provided in the command. 

`docker-compose up -d` uses the YAML configuration to deploy multiple containers together, while `-d` keeps them running in the background.

For example:

```bash
docker-compose up -d
```
