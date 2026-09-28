# Docker Compose Guide

## The services: Block

The `services:` block defines the containers that make up the application. Each service represents a separate container with its own image, configuration, environment variables, and other settings.

In this project, there are two services:

- `database` - runs the MariaDB database.
- `app` - runs the Nextcloud application.

## What does the services: block do? 
The services: block defines the different containers that make up the application. In this project, it contains two services: the database service running MariaDB and the app service running Nextcloud.

## How did the Nextcloud app container know how to find the database container?
The Nextcloud container uses the MYSQL_HOST environment variable:
```yaml
- MYSQL_HOST=database




