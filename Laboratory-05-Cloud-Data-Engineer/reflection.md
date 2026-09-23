# Mission Reflection

Object storage is better suited for storing millions of photos because it is designed to handle large amounts of unstructured data. Unlike a traditional block storage hard drive, object storage stores each photo as an individual object with its own metadata and identifier. It can also scale as the number of photos increases, which makes it useful for a photo-sharing application.

Using Docker made it easier to deploy the MinIO storage server because I did not need to manually install and configure all of the required components. With one Docker command, I was able to download the MinIO image, create a container, configure the ports, and set the administrator credentials. This made the deployment process faster and easier to repeat.

A bucket is a container in object storage where objects such as photos, videos, and documents are stored. In this activity, I created a bucket named "client-photos" to represent the storage area for the user's uploaded images. It helps organize the objects stored in MinIO.

Large enterprise companies can protect their object storage data from physical server crashes by keeping multiple copies of the data. They can use replication, backups, redundancy, and storage across different servers or locations. This means that if one physical server fails, another copy of the data can still be available.

My confidence in navigating the Linux command line is growing because I was able to use commands to deploy and check the MinIO Docker container. At first, the Docker command was confusing, especially when I encountered an error. However, after correcting the command and checking the container with "docker ps", I understood the process better. I am becoming more comfortable using the terminal and understanding what the commands do instead of simply copying them.
