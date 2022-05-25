FROM php:8.1-fpm
RUN apt-get update && apt-get install -y --no-install-recommends \
      libicu-dev \
    && rm -rf /var/lib/apt/lists/* \
    && docker-php-ext-install opcache \
    && docker-php-ext-install intl \
    && docker-php-ext-install pdo_mysql \
    && docker-php-ext-install bcmath
