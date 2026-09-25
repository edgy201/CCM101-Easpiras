# Cloud Storage Types Research

## Comparison of Storage Types

| Feature / Aspect | Block Storage | File Storage | Object Storage |
| :--- | :--- | :--- | :--- |
| **Description** | Divides data into raw, unformatted volumes or fixed-size blocks managed by an OS. | Stores data in a hierarchical file and folder structure accessed over a network protocol (NFS/SMB). | Stores data as discrete objects in a flat namespace along with custom metadata and a unique ID. |
| **Primary Use Case** | Virtual machine boot disks, relational databases, performance-critical workloads. | Shared network file drives, legacy application storage, content management systems. | Unstructured data storage (images, videos, backups, static web assets, logs). |
| **Cloud Example** | Amazon EBS (Elastic Block Store) | Amazon EFS (Elastic File System) | Amazon S3 (Simple Storage Service) |

---

## Storage Recommendation for Client Web Application

Object Storage is the ideal choice for storing your user-uploaded images because web application containers are ephemeral and should not retain state locally. Object Storage provides unlimited scalability without requiring server disk resizing, allowing seamless growth to millions of files. Additionally, it offers direct HTTP/S REST API accessibility, which simplifies secure image delivery directly to end-user web applications.
