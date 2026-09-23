# Cloud Storage Types Research

Storage Type| Description| Primary Use Case| Cloud Provider Example
Block Storage| Stores data in separate blocks. It works like a virtual hard drive that can be attached to a computer or virtual machine.| Databases, operating systems, and virtual machines| AWS EBS
File Storage| Stores data as files and folders, similar to how files are organized on a normal computer.| Shared files and folders between different users or servers| AWS EFS
Object Storage| Stores data as objects together with information or metadata about each object.| Photos, videos, backups, and other large amounts of unstructured data| Amazon S3

Why Object Storage is Suitable for User-Uploaded Images

Object Storage is a good choice for the photo-sharing application because it can store a very large number of images and can easily scale as more users upload photos. It is also designed for unstructured data such as images and videos, making it more suitable than traditional storage for this type of application.
