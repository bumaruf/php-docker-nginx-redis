FROM php:8-fpm-alpine

RUN apk update --no-cache && apk add \
libxml2-dev \
icu-dev \
oniguruma-dev \
tzdata \
libmcrypt-dev

RUN apk add --no-cache --virtual .build-deps \
g++ make autoconf yaml-dev

RUN pecl install redis \
pecl install xdebug \
pecl install mcrypt

RUN docker-php-ext-install intl
RUN docker-php-ext-install pcntl
RUN docker-php-ext-install pdo_mysql
RUN docker-php-ext-install mysqli
RUN docker-php-ext-install mbstring
RUN docker-php-ext-install calendar
RUN docker-php-ext-install sockets

RUN docker-php-ext-enable redis.so
RUN docker-php-ext-enable xdebug
RUN docker-php-ext-enable mcrypt.so

RUN rm -rf /var/cache/apk/*

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin --filename=composer

COPY php.ini /usr/local/etc/php/php.ini

CMD ["php-fpm"]
