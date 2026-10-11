# Laboratory 07 – Cloud Operations Engineer

## Mission Overview

This laboratory focuses on monitoring a Linux host system and a Docker container. The activity uses the KillerCoda Ubuntu Playground to inspect system resources, deploy an Nginx web server, generate HTTP traffic, analyze application logs, and monitor container performance.

## Objectives

- Establish the host system's RAM and disk storage baseline.
- Monitor CPU activity and running processes.
- Deploy an Nginx container using Docker.
- Generate successful HTTP requests and a 404 error.
- Analyze application logs to identify HTTP responses.
- Monitor CPU, memory, and network usage.
- Document the results and reflect on cloud operations practices.

## Monitoring Commands Executed

| Command | Purpose |
|---|---|
| `free -h` | Check RAM usage and total memory |
| `df -h /` | Check root filesystem storage |
| `top` | Monitor CPU activity and running processes |
| `docker run -d --name client-website -p 8080:80 nginx` | Deploy the Nginx container |
| `docker ps` | Verify running containers |
| `curl http://localhost:8080/` | Test website access |
| `curl -i http://localhost:8080/hidden-admin-page` | Generate and inspect a 404 response |
| `docker logs client-website` | Review application logs |
| `docker stats` | Monitor real-time container metrics |

## Skills Learned

- Linux system resource monitoring
- Docker container deployment and management
- HTTP request testing using curl
- Application log analysis
- Real-time CPU and memory monitoring
- Technical documentation and troubleshooting

