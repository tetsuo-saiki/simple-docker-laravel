FROM php:7.2.2-fpm-alpine3.6

ENV COMPOSER_ALLOW_SUPERUSER 1

RUN apk update && \
    docker-php-ext-install pdo_mysql mysqli mbstring && \
    curl -sS https://getcomposer.org/installer | php && \
    mv composer.phar /usr/local/bin/composer

WORKDIR /var/www/app

# RUN composer create-project laravel/laravel . "5.7.*"