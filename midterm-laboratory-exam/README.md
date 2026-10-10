
# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

This laboratory focuses on deploying a two-tier cloud application using Docker Compose. The project uses Nextcloud as the web and application tier and MariaDB as the database tier. Both services are configured in a `docker-compose.yml` file to make deployment easier.

## Objectives

* Understand the concept of a two-tier architecture.
* Learn how to create and configure a Docker Compose YAML file.
* Deploy Nextcloud and MariaDB as separate containers.
* Connect the application container to the database container.
* Use environment variables to configure database credentials and connections.
* Understand how Docker Compose simplifies application deployment.

## Commands Executed

The following commands were used during the laboratory:

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker compose up -d
docker ps
docker compose logs
docker compose down
```

**Note:** The commands shown above include the main deployment and management commands. Use only the commands that you actually executed in your laboratory report.

## Skills Learned

* Creating and editing configuration files using Nano.
* Writing YAML configuration with correct indentation.
* Deploying and managing Docker containers.
* Configuring application and database services.
* Using environment variables for service configuration.
* Understanding container networking and service discovery.
* Documenting cloud deployment procedures for other engineers.

## Conclusion

This laboratory helped me understand how Docker Compose can simplify the deployment of cloud applications. I learned how to configure multiple containers, connect an application to a database, and manage services through a single configuration file.
