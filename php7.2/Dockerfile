FROM php:7.2.4-fpm-alpine

RUN mkdir -p /var/run/php-fpm

RUN rm /usr/local/etc/php-fpm.d/www.conf
ADD conf/www.conf /usr/local/etc/php-fpm.d/www.conf
