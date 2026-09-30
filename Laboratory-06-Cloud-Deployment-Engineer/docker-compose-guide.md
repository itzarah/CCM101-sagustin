## Docker Compose Guide

# 1. What does the "services:" block do?

The "services:" block defines the containers that Docker Compose will create and manage. In this project, it contains the database and app services.

# 2. How does the Nextcloud app container know how to find the database container?

The Nextcloud app finds the database through the "MYSQL_HOST" environment variable. Its value is "database", which is the name of the MariaDB service.

# 3. What is the difference between "docker run" and "docker-compose up -d"?

The "docker run" command is normally used to create and start one container. The "docker-compose up -d" command uses a Compose file to create and start multiple related containers at the same time.

# Commands Used

mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
