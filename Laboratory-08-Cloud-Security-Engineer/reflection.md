# Mission Reflection

Completing Laboratory 08 helped me understand the importance of protecting cloud servers through proper firewall configuration and security practices. I learned that deploying an application is not enough because the server must also be protected from unauthorized access.

A host-based firewall protects a server by controlling incoming and outgoing network traffic directly on the machine. Even if an attacker bypasses the physical network perimeter, the firewall can still block unauthorized connections based on its configured rules. This provides another layer of security and helps protect services running on the server.

Managing open network ports is also important because every unnecessary port can become a potential entry point for attackers. By allowing only the ports required by legitimate services, administrators can reduce the server's attack surface. In this activity, I allowed SSH on port 22 for administration and TCP port 8080 for the Nginx web application while applying a default-deny policy to incoming traffic.

In a real enterprise environment, leaving a database port such as MySQL's port 3306 open to the public internet is dangerous. Attackers could attempt to exploit vulnerabilities, guess credentials, or access sensitive information if other security controls fail. Database access should instead be restricted to trusted application servers, authorized administrators, and approved network sources.

This mission changed my perspective on how easily a server can become exposed when security settings are overlooked. I realized that even a simple web application needs proper access controls, firewall rules, and regular security checks. I also learned why SSH must be allowed before enabling a firewall on a remotely managed server.

Finally, having eight completed missions in my GitHub portfolio gives me a clearer record of my progress in cloud computing. Each mission helps me develop practical skills in deployment, networking, storage, operations, and security. My portfolio also demonstrates my ability to document commands, organize project files, capture evidence, and explain what I have learned. Overall, this activity strengthened my understanding of the role of security in maintaining reliable and protected cloud infrastructure.
