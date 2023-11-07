# jenkins-nginx-reverse-proxy

* Add your SSL Certificate to the `nginx/ssl/examplecom.crt` file.
* Add your SSL Key to the `nginx/ssl/examplecom.key` file.

Creating the `jenkins/data` directory :
```sh
mkdir -p jenkins/data
```
Define 777 `[rwx]` permissions to the `jenkins/data` folder to avoid permission problems when Jenkins runs.
```sh
chmod -R 777 jenkins/data
```

We can run the compose file to stand up the containers:
```sh
docker compose up --build -d
```