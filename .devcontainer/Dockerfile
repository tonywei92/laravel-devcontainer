FROM mcr.microsoft.com/devcontainers/php:1-8.2-bullseye

# Install required packages and PHP extensions
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get install -y libpq-dev libpng-dev libzip-dev imagemagick \
    && docker-php-ext-install pdo pdo_pgsql \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/*