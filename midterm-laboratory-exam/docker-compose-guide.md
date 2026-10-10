
# Docker Compose Guide

## 1. What Does the `services:` Block Do?

The `services:` block defines the containers that make up the application. In our project, we used two services: `database` and `app`.

* **Database Service:** Uses the `mariadb:10.6` image to store Nextcloud data, user accounts, and other information.
* **App Service:** Uses the `nextcloud` image to run the Nextcloud application and provide its web interface.

Docker Compose allows us to define and manage both services in one YAML file instead of configuring each container separately.

## 2. How Does Nextcloud Find the Database?

The Nextcloud application connects to the database through the `MYSQL_HOST` environment variable.

In our `docker-compose.yml` file, we used:

```yaml
MYSQL_HOST=database
```

The word `database` matches the name of the database service defined under `services:`. Docker Compose creates a shared network for the services, allowing the Nextcloud container to find the database using its service name.

This makes communication between the application and database easier without manually entering the database container's IP address.

Other environment variables, such as `MYSQL_PASSWORD`, provide the credentials needed to connect to the database.

## 3. Difference Between `docker run` and `docker-compose up -d`

**`docker run`**

The `docker run` command starts an individual container using the options provided in the terminal. When an application needs multiple containers, we may need to run several commands and configure their connections separately.

**`docker-compose up -d`**

The `docker-compose up -d` command starts the services defined in the `docker-compose.yml` file in detached mode, meaning they run in the background. Modern Docker installations may use `docker compose up -d` with a space instead.

Docker Compose reads the configuration file and manages the services, networks, and other defined settings together.

## Conclusion

Docker Compose makes deploying multi-container applications easier, more organized, and repeatable. By defining the Nextcloud application and MariaDB database in one YAML file, we can start and manage the complete system using a single command.
