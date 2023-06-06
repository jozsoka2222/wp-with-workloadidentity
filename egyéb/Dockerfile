FROM wordpress:latest

# Install necessary packages
RUN apt-get update && apt-get install -y \
    zlib1g-dev \
    && docker-php-ext-install zip

# Install Redis PHP extension
RUN pecl install redis && docker-php-ext-enable redis
