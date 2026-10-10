# Laboratory 04 – Cloud-Native Engineer

## Mission Overview

This laboratory activity introduced cloud-native concepts by comparing virtual machines and containers and practicing basic Docker operations. The activity used Docker to pull, run, verify, manage, and remove an Nginx container.

## Objectives

* Understand the difference between virtual machines and containers.
* Verify that Docker is installed and running.
* Pull and run an official Nginx Docker image.
* Map a host port to a container port.
* Manage the container lifecycle using Docker commands.
* Document Docker activities using Markdown.

## Docker Commands Executed

### Checkpoint 3 – Verify Docker

```bash
docker --version
docker info
```

### Checkpoint 4 – Deploy Nginx

```bash
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
curl http://localhost:8080
```

### Checkpoint 5 – Container Lifecycle

```bash
docker ps
docker stop nginx-server
docker ps
docker ps -a
docker rm nginx-server
docker ps -a
```

## Skills Learned

I learned how to use Docker commands to check the Docker environment, download images, run containers, verify a web server, and manage container lifecycles. I also learned how port mapping allows a containerized web server to be accessed from the host computer.

## Challenges Encountered

One challenge was understanding the different Docker commands and their purposes. I also needed to verify that the Nginx container was running correctly before stopping and removing it.
