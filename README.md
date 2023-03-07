# Docker laravel starter
A simple docker compose workflow for local laravel deverlopment

## Usage
To get started, make sure you have [Docker installed](https://docs.docker.com/docker-for-mac/install/) on your system, and then clone this repository.

Next, navigate in your terminal to the directory you cloned this, and spin up the containers by running `docker-compose up -d --build`.

## Services
- **app** - `php and composer container`
- **nginx** - `:8001,:4431`
- **db** - `:33061`
- **redis** - `:`
- **mailhog** - `:1125,8125`
- **elasticsearch** - `:9201`
- **kinaba** - `:5601`

## Executing commands on a container
`docker-compose exec {container_name} command` example install composer on app container `docker-compose exec app composer install`