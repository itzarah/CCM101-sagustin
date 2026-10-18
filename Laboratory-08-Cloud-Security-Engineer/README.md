# Mission Overview

This laboratory activity focuses on securing a Linux server using the UFW firewall. I deployed an Nginx web application and configured firewall rules to control incoming network traffic.

### Objectives

- Understand the Principle of Least Privilege.
- Identify the attack surface of a server.
- Configure a Default Deny firewall policy.
- Allow SSH and web application traffic through specific ports.
- Document security configurations using Markdown.

### Commands Executed

docker --version
docker run -d --name secure-web-app -p 8080:80 nginx
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered

### Skills Learned

Through this activity, I learned how to deploy a web application using Docker, configure a Linux firewall, manage network ports, and document server security settings. I also learned why it is important to allow only the services required by a server.

