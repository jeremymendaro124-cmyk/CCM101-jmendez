# Multi-Tier Architecture

## Two-Tier Architecture

A Two-Tier Architecture is a system design that separates an application into two main layers: the Web/Application Tier and the Database Tier. Each tier performs a specific function and communicates with the other tier to provide the complete application service.

## The Web/Application Tier

The Web/Application Tier is responsible for providing the application's user interface and handling HTTP requests from users. In this laboratory, the Nextcloud container serves as the application tier and allows users to access the cloud storage system through a web browser.

## The Database Tier

The Database Tier is responsible for storing and managing persistent application data. In this deployment, the MariaDB container stores the database information required by the Nextcloud application, including user and application data.

## Why Separate Them?

Separating the web server and database into two containers makes the system easier to manage, maintain, and scale. Each container can be updated, restarted, or scaled independently without placing the entire application in a single container.
