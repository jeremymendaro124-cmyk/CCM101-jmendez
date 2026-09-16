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

Docker Commands Executed
Check Docker Installation
docker --version

Check Docker Environment
docker info

Download Nginx
docker pull nginx

Run Nginx
docker run -d -p 8080:80 --name nginx-server nginx

Test Nginx
curl http://localhost:8080

List Running Containers
docker ps

Stop the Container
docker stop nginx-server

View All Containers
docker ps -a

Remove the Container
docker rm nginx-server


## Skills Learned

I learned how to use Docker commands, deploy Nginx, map ports, and manage container lifecycles.

## Challenges Encountered

I had difficulty understanding port mapping and using the correct Docker commands. Testing Nginx with `curl` helped me confirm that the container was working.
