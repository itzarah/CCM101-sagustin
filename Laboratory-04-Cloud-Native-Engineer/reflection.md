### 1. How does the boot time and setup process of a Docker container compare to installing an operating system on a Virtual Machine?
Answer:
Docker containers are generally much faster to start than Virtual Machines. A VM needs to boot a complete operating system before the application can run. A container shares the host operating system kernel, so it can start in seconds. This makes containers convenient for quickly deploying applications.

### 2. Why is port mapping -p 8080:80 necessary?
Answer:
Port mapping connects port 8080 on the host machine to port 80 inside the container. Nginx listens on port 80 inside the container, while port 8080 allows us to access the web server from the host. Without the mapping, the Nginx service may not be accessible through the host's port 8080.

### 3. What happens to the data inside a container when you use docker rm?
Answer:
The docker rm command removes the container itself and its writable container filesystem. Data stored only inside that container can therefore be lost. Data that needs to remain after removing a container should be stored using persistent storage such as Docker volumes.

### 4. How do you think containerization changes the way software developers and IT operations teams work together?
Answer:
Containerization can make collaboration between developers and IT operations easier because applications and their dependencies can be packaged consistently. Developers can test the same containerized application that operations teams deploy. This supports the DevOps approach by making development, testing, and deployment more consistent.

### 5. How is your GitHub portfolio evolving?
Answer:
My GitHub portfolio is becoming more organized as I add each laboratory activity. In this activity, I added documentation about virtualization and containers, Docker deployment commands, screenshots, and a reflection. It shows my progress in learning cloud computing and practical cloud-native technologies.
My GitHub portfolio is becoming more organized as I add each laboratory activity. In this activity, I added documentation about virtualization and containers, Docker deployment commands, screenshots, and a reflection. It shows my progress in learning cloud computing and practical cloud-native technologies.
