FROM php:apache
RUN apt-get update && apt-get install -y \
    vim \
	zip unzip
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer
COPY composer.json /var/www/html
WORKDIR /var/www/html
