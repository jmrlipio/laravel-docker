# laravel-docker
A docker wrapper for Laravel with NPM, ARTISAN & COMPOSER command

1. Create src & mysql folder after cloning this repo.

# Commands:
### Check docker status

-> sudo systemctl status docker

### Enable docker

-> sudo systemctl enable --now docker

### build docker

docker-compose up -d --build

### down docker

-> docker-compose down

### run artisan command in docker

-> docker-compose run --rm artisan migrate

### run composer command in docker

-> docker-compose run --rm composer 

### run artisan npm in docker

-> docker-compose run --rm npm

### get ip address of container

-> docker inspect CONTAINER_ID | grep "IPAddress"
