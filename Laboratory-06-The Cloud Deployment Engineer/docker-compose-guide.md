### 1. What does the `services:` block do?

The `services:` block defines the **containers or services** that Docker Compose will create and run. In the YAML file, there are two services: **`database`** for MariaDB and **`app`** for Nextcloud. It allows both containers to be managed together as one application.

### 2. How did the Nextcloud app container know how to find the database container?

The Nextcloud container uses the environment variable:

```yaml
MYSQL_HOST=database
```

The value **`database`** matches the service name of the MariaDB container:

```yaml
database:
  image: mariadb:10.6
```

Docker Compose automatically creates a network for the services, so the Nextcloud app can use **`database` as the hostname** to communicate with the MariaDB container.

### 3. What is the difference between `docker run` and `docker-compose up -d`?

`docker run` is normally used to **create and start one container at a time**. You need to specify the image and options for that particular container.

`docker-compose up -d`, on the other hand, reads the **`docker-compose.yml` file** and creates and starts **multiple related services together**. In this activity, it can start both the Nextcloud app and MariaDB database with their required settings and networking.