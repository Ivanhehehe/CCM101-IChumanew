# Types of Cloud Storage

Cloud storage can be divided into three primary types: Block Storage, File Storage, and Object Storage. Each type stores and manages data differently and is suited for different applications.

| Storage Type       | Description                                                                                                                              | Primary Use Case                                                                               | Cloud Provider Example              |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ----------------------------------- |
| **Block Storage**  | Stores data in fixed-size blocks that can be accessed individually. It works like a virtual hard drive attached to a computer or server. | Best for operating systems, databases, and applications that need fast and direct data access. | **AWS EBS (Elastic Block Store)**   |
| **File Storage**   | Stores data as files organized into folders and directories. Multiple users or systems can access the same file system over a network.   | Best for shared files, documents, and applications that need a common file system.             | **AWS EFS (Elastic File System)**   |
| **Object Storage** | Stores data as objects together with metadata and a unique identifier. It is designed to store large amounts of unstructured data.       | Best for images, videos, backups, documents, and other large collections of unstructured data. | **AWS S3 (Simple Storage Service)** |

### Why Object Storage is Best for the Client

Object Storage is the best choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as user-uploaded images. It can organize millions of photos as objects and provide scalable access to the stored files without depending on the web server's local storage.
