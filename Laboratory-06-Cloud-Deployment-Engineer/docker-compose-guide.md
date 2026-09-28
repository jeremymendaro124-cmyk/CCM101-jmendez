# Docker Compose Guide

## The `services:` Block

The `services:` block defines the containers that make up the application. Each service represents a separate container with its own image and configuration.

In this project, there are two services:

* `database` - runs the MariaDB database.
* `app` - runs the Nextcloud application.

## How Does Nextcloud Find the Database?

The Nextcloud application finds the database through the `MYSQL_HOST` environment variable:

```yaml
- MYSQL_HOST=database
```

The value `database` is the name of the database service. Docker Compose allows the containers to communicate using their service names.

## Difference Between `docker run` and `docker-compose up -d`

`docker run` is used to create and start one Docker container manually. On the other hand, `docker-compose up -d` reads the `docker-compose.yml` file and starts multiple related containers at the same time.

The `-d` option runs the containers in the background.
