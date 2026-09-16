# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

This laboratory activity focuses on understanding the difference between Virtual Machines and Containers. We used Docker to deploy and manage an Nginx web server in a cloud-based playground.

## Objectives

- Differentiate Virtual Machines and Containers.
- Verify that Docker is installed and running.
- Use basic Docker commands.
- Pull and run an Nginx container.
- Manage the lifecycle of a container.
- Document Docker operations using Markdown.

## Docker Commands Executed

docker --version
docker info
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
curl http://localhost:8080
docker ps
docker stop nginx-server
docker ps
docker ps -a
docker rm nginx-server
docker ps -a

##Skills Learned
I learned how to use basic Docker commands, pull an image, run a container, check a container, stop a container, and remove a container. I also learned how to document technical procedures using Markdown and GitHub.

##Challenges Encountered
One challenge was understanding the Docker commands and the purpose of port mapping. I also needed to carefully check the terminal output to make sure that the Nginx container was running correctly.
