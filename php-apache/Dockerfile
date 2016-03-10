FROM php:7-apache

RUN apt-get update \
    && docker-php-ext-install pdo pdo_mysql \
    && docker-php-ext-install mcrypt \
    && a2enmod rewrite \
    && service apache2 restart

COPY apache2.conf /etc/apache2/apache2.conf

WORKDIR /var/www

EXPOSE 80
CMD ["apache2-foreground"]