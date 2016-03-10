FROM php:7-fpm

RUN apt-get update \
    && docker-php-ext-install pdo pdo_mysql

WORKDIR /var/www

CMD ["php-fpm"]