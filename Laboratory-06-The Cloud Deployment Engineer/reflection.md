# Reflection

Working with Docker Compose helped me understand how cloud engineers can manage applications more efficiently. Instead of manually typing several `docker run` commands with different options, a cloud engineer can define the application's configuration in a `docker-compose.yml` file. This makes the deployment process more organized, repeatable, and easier to manage. Once the configuration is prepared, the services can be started with a single command such as `docker compose up -d`.

I also learned that YAML files are sensitive to indentation. YAML uses spaces to organize its structure, so an indentation error, such as using a Tab instead of Spaces, can cause a parsing error. When this happens, Docker Compose may fail to read the configuration file and the services will not start properly. This showed me that even small formatting mistakes can affect the entire deployment process.

Environment variables such as `MYSQL_PASSWORD` were used to provide configuration information needed by the containers. In our Compose file, these variables helped configure the connection between the Nextcloud application and the MariaDB database. Using environment variables also keeps configuration values separate from the application's main settings and makes the deployment easier to modify.

Deploying Nextcloud in only a few minutes was a meaningful experience for me. It showed me how powerful containerization can be because a system that would normally require several installation and configuration steps could be deployed quickly using predefined containers.

Since Mission 1, my understanding of Cloud Computing has evolved significantly. I initially viewed cloud computing mainly as accessing resources and services over the internet. Through the succeeding missions, I learned that cloud computing also involves infrastructure, virtualization, networking, storage, containers, automation, and service management. I now have a better understanding of how cloud engineers use tools such as Linux, Docker, and Docker Compose to build and deploy reliable applications efficiently.
