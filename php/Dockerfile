FROM php:8.1-apache
RUN docker-php-ext-install mysqli && \
    docker-php-ext-enable mysqli

RUN apt-get update -y && apt-get install -y sendmail libpng-dev
RUN apt-get update -y && apt-get install -y zlib1g-dev libzip-dev libicu-dev

RUN docker-php-ext-install gd && \
    docker-php-ext-enable gd
RUN docker-php-ext-install zip && \
    docker-php-ext-enable zip
RUN docker-php-ext-install exif && \
    docker-php-ext-enable exif
RUN docker-php-ext-install intl && \
    docker-php-ext-enable intl
RUN a2enmod rewrite