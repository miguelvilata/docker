FROM php:7.2-fpm
  
RUN pecl install xdebug-2.6.0 \
    && docker-php-ext-enable xdebug \
    && docker-php-ext-install pdo pdo_mysql

RUN apt-get update && apt-get install -y vim

COPY "./ini/php.ini-development" "/usr/local/etc/php/php.ini"    
  
