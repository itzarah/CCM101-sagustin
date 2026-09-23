# Cloud Storage Types Research

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-size blocks. | Virtual machines and databases | AWS EBS |
| File Storage | Stores data as files organized in folders/directories. | Shared files and directories | AWS EFS |
| Object Storage | Stores data as objects together with metadata and unique identifiers. | Photos, videos, backups, and other unstructured data | Amazon S3 |

## Why Object Storage for User Photos?

Object Storage is well suited for user-uploaded photos because it is designed for large amounts of unstructured data. It can store individual images as objects and can scale as the number of uploaded photos increases.
