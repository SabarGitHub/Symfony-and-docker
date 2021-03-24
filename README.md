# App Symfony 5 and docker containers

### Docker
```
git clone https://github.com/SabarGitHub/Symfony-and-docker.git

cd Symfony-and-docker

cd app

docker-compose up -d

```

### PHP (app_www)

```
cd Symfony-and-docker

cd app

docker-compose run www_app composer install

docker exec -it www_app php bin/console doctrine:migration:migrate 
```
