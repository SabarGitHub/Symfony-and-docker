FROM php:8.0.0RC3-fpm-alpine
RUN apk --update --no-cache add git
RUN docker-php-ext-install pdo pdo_mysql mysqli
COPY php.ini /usr/local/etc/php/php.ini
COPY --from=composer /usr/bin/composer /usr/bin/composer
WORKDIR /var/www/html
CMD composer install ; php-fpm

EXPOSE 9000