# MinIO Deployment Documentation

## 1. Docker Command Used

The MinIO server was deployed using Docker with the following command:

docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"

This command creates and runs a MinIO container named minio-server.

## 2. Web Console Port
The MinIO Web Console uses:
Port 9001
Port 9001 was used to access the MinIO Web Console through the KillerCoda environment.
Port 9000 is used for the MinIO API.

## 3. Bucket Created
The bucket created for the application is:
client-photos
This bucket is intended to store user-uploaded images for the photo-sharing application.

## 4. Environment Variables
The -e flags in the Docker command are used to set environment variables inside the MinIO container.
The following environment variables were used:
MINIO_ROOT_USER=cloudadmin — sets the MinIO administrator username.
MINIO_ROOT_PASSWORD=CloudNova2026! — sets the MinIO administrator password.
These variables provide the login credentials used to access the MinIO Web Console.

## 5. Deployment Verification
The MinIO container was checked using the following command:
docker ps
