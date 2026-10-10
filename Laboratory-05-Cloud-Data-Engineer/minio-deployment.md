# MinIO Deployment

## Docker Command Used

The laboratory provided the following Docker command for deploying the MinIO object storage server:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
```

The command was attempted in the KillerCoda Ubuntu Playground. However, the `minio/minio` image could not be downloaded because access to the archived repository was denied by the Docker environment.

## Port Used for the Web Console

The MinIO Web Console uses port **9001**.

Port **9000** is used for the MinIO API, while port **9001** is used for the web-based management console.

## Bucket Name

The required bucket name for this laboratory activity is:

`client-photos`

The bucket could not be created because the MinIO Web Console could not be accessed successfully in the provided environment.

## Environment Variables

The `-e` flags in the Docker command define environment variables inside the container.

* `MINIO_ROOT_USER=cloudadmin` sets the administrator username.
* `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the administrator password.

These environment variables provide the login credentials for the MinIO server.

## Deployment Issue

The provided laboratory instructions use the `minio/minio` Docker image. During deployment, Docker returned an access-denied error when attempting to pull the image. An alternative current MinIO image was also tested, but it required a license, so it could not be used to complete the laboratory's bucket and upload requirements.

Therefore, the deployment could not be fully completed in the available KillerCoda environment.
