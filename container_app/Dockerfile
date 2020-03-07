FROM php:apache
RUN apt-get update && apt-get install -y \
    vim
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer
COPY composer.json /tmp

