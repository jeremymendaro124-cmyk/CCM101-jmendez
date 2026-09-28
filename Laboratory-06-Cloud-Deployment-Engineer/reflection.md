# Mission Reflection

Writing a `docker-compose.yml` file makes a cloud engineer's job easier because it allows multiple containers and their configurations to be defined in one file. Instead of manually typing several Docker commands, the engineer can use `docker-compose up -d` to deploy the entire application stack. This makes the deployment process faster, more organized, and easier to reproduce.

YAML is sensitive to indentation, so an indentation error can cause the Compose file to fail when Docker tries to read it. Using a Tab instead of spaces or placing an item at the wrong indentation level can result in a YAML parsing error. This shows why proper formatting is important when writing infrastructure configuration files.

Environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` were used to provide configuration information to the containers. They allow the application and database to share the required settings without placing these values directly inside the application code. In this activity, the `MYSQL_HOST=database` variable also allowed the Nextcloud application to locate the MariaDB database container through its service name.

Deploying Nextcloud was an interesting experience because a functional cloud storage platform could be prepared within only a few minutes using containers. The activity demonstrated how Docker can simplify the deployment of applications that normally require several installation and configuration steps.

Since Mission 1, my understanding of Cloud Computing has evolved from learning basic cloud concepts to understanding how cloud infrastructure can actually be created and deployed. I now have a better understanding of virtualization, containers, cloud services, networking, storage, and automated deployment. This mission also showed me that cloud engineers can use configuration files to make infrastructure deployment more consistent, efficient, and easier to manage.
