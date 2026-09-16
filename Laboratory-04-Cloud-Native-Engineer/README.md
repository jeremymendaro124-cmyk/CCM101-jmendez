# Laboratory 04 – The Cloud-Native Engineer

## Mission Overview

This laboratory introduces Docker and containerization. It demonstrates deploying and managing an Nginx web server using KillerCoda.

## Objectives

* Understand VMs and containers.
* Check Docker installation.
* Deploy an Nginx container.
* Use port mapping.
* Manage containers.

## Docker Commands Executed

### Check Docker Installation

```bash
docker --version
```

### Check Docker Environment

```bash
docker info
```

### Download Nginx

```bash
docker pull nginx
```

### Run Nginx

```bash
docker run -d -p 8080:80 --name nginx-server nginx
```

### Test Nginx

```bash
curl http://localhost:8080
```

### List Running Containers

```bash
docker ps
```

### Stop the Container

```bash
docker stop nginx-server
```

### View All Containers

```bash
docker ps -a
```

### Remove the Container

```bash
docker rm nginx-server
```


## Skills Learned

I learned how to use Docker commands, deploy Nginx, map ports, and manage container lifecycles.

## Challenges Encountered

I had difficulty understanding port mapping and using the correct Docker commands. Testing Nginx with `curl` helped me confirm that the container was working.
