# Rclone Sync test

Le but de ce repository est de tester la commande `rclone sync` entre deux Object Storage S3 compatible.

Dans notre cas les S3 capatibles, sont des containers [Minio](https://min.io/)

## Getting-started

1. Lancer minio1 : 
```shell
docker-compose up minio1 minio2
```

2. Ajouter un bucket dans chaque minio disponible : [minio1](http://localhost:9001) et [minio2](http://localhost:9002)

3. Quand vous souhaitez essayer le sync : 
```shell
docker-compose up rclone
```
