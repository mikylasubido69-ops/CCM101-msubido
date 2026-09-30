# Laboratory 06 – Cloud Deployment Engineer

## Mission Overview

This laboratory focused on deploying a multi-container application using **Docker Compose**. The activity involved creating a YAML configuration file that defines a Nextcloud application container and a MariaDB database container. The goal was to understand how multiple containers can work together as a single cloud-based application.

## Objectives

* Understand the basic structure of a Docker Compose YAML file.
* Create and configure multiple services using Docker Compose.
* Deploy a Nextcloud application with a MariaDB database.
* Understand how containers communicate with each other.
* Use environment variables to configure database connectivity.
* Learn the difference between `docker run` and `docker-compose up -d`.
* Practice managing a multi-container application.

## Commands Executed

The following commands were used during the laboratory activity:

```bash
docker --version
docker compose version
docker compose up -d
docker compose ps
docker compose logs
docker compose down
```

The main deployment command was:

```bash
docker compose up -d
```

This command reads the `docker-compose.yml` file and starts the configured services in detached mode.

To check the running containers:

```bash
docker compose ps
```

To stop and remove the containers created by Compose:

```bash
docker compose down
```

## Skills Learned

Through this laboratory activity, I learned how to:

* Create a Docker Compose configuration using YAML.
* Define multiple services under the `services:` block.
* Configure a Nextcloud application and MariaDB database.
* Connect containers using Docker Compose service names.
* Use environment variables such as `MYSQL_HOST` for database connectivity.
* Deploy multiple containers using a single command.
* Monitor and manage containers using Docker Compose commands.
* Understand the difference between running an individual container with `docker run` and deploying multiple services with `docker compose up -d`.
* Apply containerization concepts to a multi-tier cloud application.
