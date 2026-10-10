
# Mission Reflection - Laboratory 06

During this laboratory, I learned how to deploy Nextcloud using Docker Compose and connect it to a MariaDB database. This activity helped me understand cloud deployment better and showed me how useful Docker can be when managing applications.

**1. How does writing a docker-compose.yml file make a cloud engineer's job easier?**

Writing a `docker-compose.yml` file makes the job easier because all the container configurations are saved in one file. Instead of typing many commands manually, I can use one command to start the application and its database. It also makes the deployment easier to repeat and manage.

**2. What happens if you make an indentation error in a YAML file?**

If I make an indentation error, such as using a Tab instead of spaces, Docker Compose may fail to read the file and display an error. YAML depends on proper spacing to organize its settings. I learned that checking the indentation is important before running the deployment.

**3. Why did we use environment variables like MYSQL_PASSWORD?**

We used environment variables to provide the database configuration and credentials needed by the containers. They help separate configuration values from the application setup and make it easier to change settings. However, passwords should still be protected and should not be exposed in public files or repositories.

**4. How did it feel to deploy Nextcloud in just a few minutes?**

I felt happy and surprised that I could deploy a cloud storage application in just a few minutes. At first, the configuration looked complicated, but Docker Compose made the process more manageable. It was satisfying to see how containers can work together to provide a useful application.

**5. How has my understanding of Cloud Computing evolved since Mission 1?**

Since Mission 1, my understanding of cloud computing has improved. I now understand that cloud computing involves more than just storing files online. It also includes deploying applications, managing services, connecting databases, and configuring networks. This laboratory helped me see how containerization makes cloud deployment more efficient and organized.

## Conclusion

Overall, this laboratory improved my understanding of Docker, Docker Compose, and multi-tier architecture. I learned that proper configuration, correct YAML indentation, and secure handling of credentials are important when deploying cloud applications. These skills will be useful in future cloud computing activities and projects.
