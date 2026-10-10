# Mission Reflection

This laboratory activity helped me understand the difference between virtual machines and Docker containers. A Docker container has a much faster boot and setup process compared to installing an operating system on a Virtual Machine. A VM needs to create virtual hardware and install or start a complete operating system, while a container can start an application using an existing Docker image. This makes containers useful when applications need to be deployed quickly.

Port mapping such as `-p 8080:80` is necessary because it connects a port on the host computer to a port inside the container. In this activity, Nginx runs on port 80 inside the container, while port 8080 on the host allows us to access the web server using `http://localhost:8080`. Without the port mapping, the web server may not be directly accessible from the host.

When the `docker rm` command is used, the container itself is permanently removed. Any data stored only inside the container that was not saved using a volume or another external storage method can also be lost. This shows why persistent data should be stored outside the temporary container when necessary.

Containerization can also improve collaboration between software developers and IT operations teams. Developers can package applications with their required environment, while operations teams can deploy the same container consistently. This supports DevOps by making development, testing, and deployment more consistent.

My GitHub portfolio is also evolving as I add more laboratory activities and technical documentation. Instead of only uploading finished projects, I am now documenting commands, screenshots, challenges, and skills learned. This makes my portfolio a better record of my progress and practical cloud computing experience.
