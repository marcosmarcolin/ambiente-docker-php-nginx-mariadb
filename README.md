# Ambiente de desenvolvimento com Docker + PHP FPM 8.1.x + Composer + Nginx + MariaDB

## Requisitos

* Docker
* Docker compose

## Docker

Crie um arquivo `.env` com o conteúdo de `.env-sample`.

### Buildar os Containers:

`docker-compose up -d --build`

### Parar todos os Containers:

`docker-composer down -v`

### Remover todos os Containers parados:

`docker system prune`

### Acessar o Container do MariaDB e ter acesso ao banco:

`docker exec -it mariadb bash`

### Acessar aplicação:

`localhost:8888`

# Composer

## Instalar

`docker-compose run --rm php-fpm composer install `

## Requerir pacote:

`docker-compose run --rm php-fpm composer require autor/pacote`