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
