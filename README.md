# Docker nginx and php-fpm with the distribuition Alpine
### Starting with Docker
    docker-compose up --build 
### Starting with Docker Run containers in the background
    docker-compose up --build up -d
## Extra commands
### To enter in container nginx
    docker exec -it webserver-alpine /bin/sh
### To enter in container php-fpm    
    docker exec -it php-fpm-alpine /bin/sh
## ENVIROMENT
    #----------------------------#
    # Configuração das Variáveis #
    #----------------------------#
    WORKING_DIR=/var/www
    #----------------------#
    # APPLICATION          #
    #----------------------#
    APPLICATION_DIR=./application
    APPLICATION_NAME=application
    #-------#
    # NGINX #
    #-------#
    NGINX_VERSION=:1.17.6-alpine
    NGINX_DEFAULT_CONF=/etc/nginx/conf.d/default.conf
    NGINX_CONF=/etc/nginx/nginx.conf
    NGINX_HOST_HTTP_PORT=80
    NGINX_HOST_HTTPS_PORT=443
    #-------#
    # MYSQL #
    #-------#
    MYSQL_VERSION=
    MYSQL_DATABASE=database
    MYSQL_USER=database
    MYSQL_PASSWORD=database
    MYSQL_PORT=3306
    MYSQL_ROOT_PASSWORD=database