FROM php:7.4.5-fpm-alpine3.11

RUN apk add --no-cache bash mysql-client
RUN docker-php-ext-install pdo pdo_mysql

WORKDIR /var/www
RUN rm -rf /var/www/html

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

#RUN composer install \
#       && cp .env.example .env \
#       && php artisan key:generate \
#       && php artisan config:cache

COPY . /var/www
RUN ln -s public html

EXPOSE 9000
ENTRYPOINT ["php-fpm"]