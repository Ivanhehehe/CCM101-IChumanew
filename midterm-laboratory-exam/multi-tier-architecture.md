
Multi-Tier Architecture

What is Two-Tier Architecture?

A two-tier architecture is a system that separates an application into two main parts: the Web/Application Tier and the Database Tier. In this laboratory activity, the Web/Application Tier uses Nextcloud, while the Database Tier uses MariaDB.

The Web/Application Tier

The Web/Application Tier is responsible for providing the application that users interact with. It handles user requests and serves the Nextcloud web interface through HTTP. In this activity, the Nextcloud application runs inside its own Docker container.

The Database Tier

The Database Tier is responsible for storing persistent information used by the application. MariaDB stores data such as user accounts and other Nextcloud-related information. It runs in a separate Docker container from the Nextcloud application.

Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage, maintain, and troubleshoot. It also allows each part of the application to be managed independently and helps organize the system into clear and separate components.
