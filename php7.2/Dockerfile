FROM php:7.2.4-fpm-alpine

RUN mkdir -p /var/run/php-fpm
RUN mkdir -p /var/run/php

RUN rm /usr/local/etc/php-fpm.d/www.conf
ADD conf/www.conf /usr/local/etc/php-fpm.d/www.conf

// https://github.com/docker-library/php/issues/279