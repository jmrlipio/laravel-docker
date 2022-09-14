# laravel-docker
A docker wrapper for Laravel with NPM, ARTISAN & COMPOSER command

1. Create src & mysql folder after cloning this repo.
2. Src folder should contain the laravel files
3. Mysql in docker-compose should be the same in laravel's .env settings


ie:

-> DB_CONNECTION=mysql

-> DB_HOST=mysql

-> DB_PORT=3306

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