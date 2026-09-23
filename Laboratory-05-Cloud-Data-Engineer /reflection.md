# Mission Reflection

This laboratory activity helped me understand how object storage can be used to manage a large amount of data in a cloud environment. Object storage is better suited for storing millions of photos because it is designed for large amounts of unstructured data. Unlike traditional block storage, object storage organizes data as individual objects with metadata and unique identifiers. This makes it easier to store, access, and manage a large collection of images as the application grows.

Using Docker made the deployment of the MinIO storage server much easier because I did not need to manually install and configure all of the required components. With a single Docker command, I was able to download the MinIO image, create a container, configure the administrator credentials, and expose the required ports. Docker also made the deployment more consistent and easier to reproduce in another environment.

A bucket in cloud storage is a container used to organize and store objects such as images, videos, documents, and other files. In this activity, I created a bucket named `client-photos`, which served as the storage location for the uploaded sample file.

Large enterprise companies can protect their object storage data from physical server failures by using redundancy, replication, backups, and distributed storage systems. Data can be stored across multiple physical servers or locations so that a hardware failure does not result in permanent data loss. These methods also help improve availability and reliability.

My confidence in navigating the Linux command line is gradually growing. Through this activity, I became more comfortable using commands such as `docker run` and `docker ps`. I also learned how command-line tools can be used to deploy and monitor cloud services. Overall, this mission gave me practical experience with Docker, Linux, and object storage.
