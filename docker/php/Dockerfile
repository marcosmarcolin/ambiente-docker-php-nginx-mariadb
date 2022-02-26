FROM php:8.1-fpm-bullseye

COPY --from=composer/composer /usr/bin/composer /usr/bin/composer

RUN apt-get update && apt-get install -y libzip-dev zip unzip

EXPOSE 9000