# Laboratory 08: Cloud Security Engineer

## Mission Overview

This laboratory focuses on securing a cloud server by deploying an Nginx web application and configuring the Uncomplicated Firewall (UFW). The mission demonstrates how firewall rules control network traffic and help reduce the server's attack surface.

## Objectives

- Understand the Principle of Least Privilege.
- Identify the attack surface of a virtual machine.
- Explain the Default Deny Policy.
- Deploy an Nginx container named `secure-web-app` on port 8080.
- Configure UFW to allow SSH while denying incoming traffic by default.
- Allow TCP traffic on port 8080.
- Verify the firewall configuration and test the web application using curl.
- Document the procedures and reflect on cloud security practices.

## Commands Executed

| Command | Purpose |
|---|---|
| `docker --version` | Check the Docker version. |
| `docker run -d --name secure-web-app -p 8080:80 nginx` | Deploy the Nginx container. |
| `curl http://localhost:8080` | Test the web application. |
| `sudo ufw allow ssh` | Allow SSH traffic. |
| `sudo ufw default deny incoming` | Block incoming traffic by default. |
| `sudo ufw default allow outgoing` | Allow outgoing traffic. |
| `sudo ufw enable` | Activate the firewall. |
| `sudo ufw status verbose` | Check firewall status and policies. |
| `sudo ufw allow 8080/tcp` | Allow TCP port 8080. |
| `sudo ufw status numbered` | Display numbered firewall rules. |

## Skills Learned

- Basic Docker container deployment.
- Testing web applications using curl.
- Configuring UFW firewall rules.
- Applying the Default Deny security policy.
- Managing SSH and web application ports.
- Documenting cloud security procedures.
- Capturing and organizing technical evidence.


