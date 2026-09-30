# Multi-Tier Architecture

## What is Two-Tier Architecture?

A **Two-Tier Architecture** is a system design that separates an application into two main parts: the **Web/Application Tier** and the **Database Tier**. In this laboratory, the Nextcloud application serves as the web/application tier, while MariaDB serves as the database tier. These components run in separate Docker containers but communicate with each other as part of the same application environment.

## The Web/Application Tier

The **Web/Application Tier** is responsible for providing the application's user interface and handling requests from users. In this activity, the **Nextcloud container** serves the web interface that users access through a browser. It also processes application requests and communicates with the database when information needs to be stored or retrieved.

## The Database Tier

The **Database Tier** is responsible for storing and managing the application's persistent information. In this activity, the **MariaDB container** stores information such as user accounts, credentials, and Nextcloud file metadata. The database provides the storage and retrieval functions needed by the Nextcloud application.

## Why Separate Them?

Separating the web application and database into two containers makes the system easier to manage, maintain, and troubleshoot because each container has a specific responsibility. It also allows the application and database to be managed or scaled independently instead of putting all components into one container. Docker recommends separating application components into different containers when they have different responsibilities.

