### Reflection

In this laboratory activity, I learned that protecting a cloud server requires more than simply running an application. A host-based firewall provides an additional layer of security by controlling the network traffic entering and leaving a server. Even if the network perimeter is breached, the firewall can still block unauthorized connections based on its configured rules.

Managing open network ports is also important because every unnecessary open port can become a possible entry point for attackers. By allowing only the ports needed by the application, administrators can reduce the server's attack surface. In this activity, I allowed SSH for remote administration and port 8080 for the Nginx web application while applying a default deny policy to incoming traffic.

In a real enterprise environment, leaving a database port such as MySQL's port 3306 open to the public internet can be dangerous. Attackers may attempt to guess passwords, exploit database vulnerabilities, or gain unauthorized access to sensitive information. Database services should generally be restricted to trusted networks and authorized application servers instead of being exposed to everyone.

This mission changed my perspective on server security because I realized that a newly deployed server can have security risks if its firewall and network access are not configured properly. Even a simple application needs protection, regular monitoring, and appropriate access controls. I also learned the importance of checking firewall status and verifying that the required rules are active.

Finally, having eight completed missions in my GitHub portfolio helps me organize my laboratory activities and demonstrate the skills I have practiced. My portfolio can serve as evidence of my learning in cloud computing, deployment, system administration, and security. I still need to continue improving my documentation and technical skills, but each mission helps me become more confident in working with cloud technologies.
