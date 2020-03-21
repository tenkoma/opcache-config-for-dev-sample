FROM php:7.4-fpm
RUN apt-get update && apt-get install -y --no-install-recommends \
      libicu-dev \
    && rm -rf /var/lib/apt/lists/* \
    && docker-php-ext-install intl \
    && docker-php-ext-install pdo_mysql \
    && pecl install xdebug \
    && docker-php-ext-enable xdebug
