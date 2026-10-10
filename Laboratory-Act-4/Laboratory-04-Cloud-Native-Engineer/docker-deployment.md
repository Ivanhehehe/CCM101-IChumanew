## Container Lifecycle

### 1. List Running Containers

```bash
docker ps
```

This command lists all currently running Docker containers.

### 2. Stop the Running Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container without removing it.

### 3. Verify the Container Is Stopped

```bash
docker ps -a
```

This command displays all containers, including stopped containers, allowing us to verify that `nginx-server` has stopped.

### 4. Remove the Container Completely

```bash
docker rm nginx-server
```

This command permanently removes the stopped `nginx-server` container.

### Lifecycle Summary

The container was first listed, then stopped, verified as stopped, and finally removed from Docker.
