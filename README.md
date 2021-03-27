# Rclone Sync test

Le but de se repository est de tester la commande `rclone sync` entre deux Object Storage S3 compatible.

Dans notre cas les S3 capatibles, sont des containers [Minio](https://min.io/)

## Getting-started

1. Lancer les minio : 
```shell
docker-compose up minio1
```

2. Récupérer l'endpoint : 

La sortie du terminal devrait afficher une ligne dans ce style :
```shell
 Endpoint: http://192.168.160.4:9000  http://127.0.0.1:9000 
```

Votre endpoint est donc : `http://192.168.160.4:9000`

3. Remplacer l'endpoint dans le fichier `rclone.conf`

4. Faire de même avec minio2 

5. Ajouter un bucket dans chaque minio et adapter le service `rclone` dans le `docker-compose.yaml``
