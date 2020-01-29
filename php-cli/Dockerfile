FROM php:7.2-cli

RUN pecl install xdebug-2.6.0 \
    && docker-php-ext-enable xdebug \
    && docker-php-ext-install pdo pdo_mysql 

RUN apt-get update && apt-get install -y default-mysql-client && rm -rf /var/lib/apt    
RUN apt-get update && apt-get install -y vim
