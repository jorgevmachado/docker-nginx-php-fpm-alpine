FROM php:7-fpm-alpine
MAINTAINER Jorge Vieira <jorge.vieira@clubemontreal.com.br>
RUN apk add --no-cache zip libzip-dev && docker-php-ext-install zip mysqli pdo pdo_mysql
