FROM php:8.4-fpm

# update and install dependencies
RUN apt-get update && apt-get install -y \
    libpq-dev \
    libzip-dev \
    curl \
    libicu-dev \
    libonig-dev \
    libxml2-dev && \
    docker-php-ext-install intl mbstring opcache zip pdo_mysql mysqli

# Install Extensions
RUN pecl install xdebug ds && docker-php-ext-enable xdebug ds

# Configure PHP
COPY ./php.ini /usr/local/etc/php/php.ini

# Configure Working Directory
WORKDIR /var/www/html

# Set permissions
RUN chown -R www-data:www-data /var/www/html
