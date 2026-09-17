# Docker Deployment

## Pull the Nginx Image

```bash
docker pull nginx
```

This downloads the official Nginx image from Docker Hub to the local Docker environment.

## Run the Nginx Container

```bash
docker run -d -p 8080:80 --name nginx-server nginx
```

This starts an Nginx container in the background and maps port 8080 on the host to port 80 inside the container.

## Test the Nginx Web Server

```bash
curl http://localhost:8080
```

This sends an HTTP request to the Nginx web server and confirms that it is running.

## List Running Containers

```bash
docker ps
```

This displays the containers that are currently running.

## Stop the Container

```bash
docker stop nginx-server
```

This stops the running Nginx container.

## Verify the Container is Stopped

```bash
docker ps -a
```

This displays all containers, including stopped containers, so the Nginx container can be checked.

## Remove the Container

```bash
docker rm nginx-server
```

This permanently removes the stopped Nginx container from the Docker environment.

## Container Lifecycle

The basic container lifecycle demonstrated in this activity was:

**Pull → Run → Test → List → Stop → Verify → Remove**
