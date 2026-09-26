## Two-Tier Architecture

# What is Two-Tier Architecture?

A two-tier architecture is a system where the application and database are separated into two different tiers. In this laboratory, the Nextcloud application works as the web/application tier, while MariaDB works as the database tier. Each tier has its own role but they communicate with each other to make the application work.

# The Web/Application Tier

The web/application tier is responsible for providing the user interface and handling HTTP requests from users. In this project, Nextcloud is the application that users access through a web browser. It processes user requests and communicates with the database when information is needed.

# The Database Tier

The database tier is responsible for storing and managing persistent data. In this project, MariaDB stores information such as user accounts, passwords, and other data needed by Nextcloud. It allows the application to save and retrieve information when needed.

# Why Separate Them?

It is better to separate the web application and database into two containers because each container can focus on its own task. This makes the system easier to manage, update, troubleshoot, and scale. If there is a problem with one container, the other container can remain separate and be managed independently.
