# Mission Reflection

This laboratory helped me understand why object storage is useful for applications that need to store a large number of files, such as photos. Object storage is better suited for millions of photos because it is designed to store large amounts of unstructured data as objects. Unlike traditional block storage, object storage organizes data into buckets and makes it easier for applications to access individual files.

Docker also makes deploying a storage server easier because the application can be packaged and started inside a container without manually installing and configuring all of its dependencies. In this activity, I learned how Docker commands can define ports, environment variables, container names, and application settings in one command. Although I was unable to complete the MinIO deployment because the required `minio/minio` image was denied by the KillerCoda environment, troubleshooting the issue helped me understand how Docker pulls images and reports registry errors.

A bucket in cloud storage is a container used to organize and store objects. In this activity, the required bucket was named `client-photos`, which represents a storage location for the client's uploaded images.

Large enterprise companies can protect object storage data from physical server failures by maintaining copies of data across different storage devices or servers. They can also use redundancy, backups, replication, and other recovery mechanisms to reduce the risk of permanent data loss.

My confidence with the Linux command line is also growing. At first, Docker commands with multiple options were unfamiliar to me, but I became more comfortable running commands, checking containers with `docker ps`, viewing images with `docker images`, and troubleshooting Docker errors. Even though the MinIO deployment could not be completed because of the environment limitation, the troubleshooting process gave me more experience working with Linux and Docker.
