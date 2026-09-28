# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

This laboratory focuses on deploying a multi-container cloud application using Docker Compose. The deployment uses Nextcloud as the web application and MariaDB as the database service.

## Objectives

* Understand Two-Tier Architecture.
* Create a multi-container Docker Compose configuration.
* Deploy Nextcloud and MariaDB containers.
* Configure communication between application and database containers.
* Access a cloud storage application through port 8080.
* Practice starting and stopping a containerized infrastructure.
* Document cloud deployment procedures.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

* Docker container deployment
* Docker Compose
* YAML configuration
* Multi-tier architecture
* Container networking
* Environment variables
* Cloud application deployment
* Infrastructure documentation
