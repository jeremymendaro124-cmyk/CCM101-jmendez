# Mission Reflection

This laboratory helped me understand how Docker containers are different from Virtual Machines. A Docker container can start within seconds because it uses the host operating system instead of installing a complete operating system. A Virtual Machine takes longer to set up because it needs virtual hardware and a full operating system before applications can be installed.

Port mapping using `-p 8080:80` is necessary because the web server runs inside the container. Port 80 is the port used by Nginx inside the container, while port 8080 allows the host machine to access it. Through port mapping, I was able to open the Nginx web server using `localhost:8080`.

When the `docker rm` command is used, the container is permanently removed. Any data stored only inside the container is also deleted. This shows the importance of using volumes or external storage when data needs to be kept after removing a container.

Containerization can improve the way developers and IT operations teams work together. Developers can package applications with their required dependencies into containers, while operations teams can deploy the same containers in different environments. This can make application deployment more consistent and easier to manage, supporting DevOps practices.

My GitHub portfolio is also improving as I complete more cloud computing laboratory activities. Each laboratory adds new skills and documentation to my repository. Laboratory 04 helped me add practical experience with Docker, containers, Nginx, port mapping, and container management. By continuing to organize and document my work, my GitHub portfolio is becoming a record of my learning and technical progress.
