#Dockerfile enter image description here A Dockerfile is a simple text file that contains the commands a user could call to assemble an image.
#Your Docker workflow should be to build a suitable Dockerfile for each image you wish to create, 
#then use compose to assemble the images using the build command.

FROM php:7.4-fpm-alpine

RUN apk update --no-cache \
&& apk add \
icu-dev \
oniguruma-dev \
tzdata
 
#RUN docker-php-ext-install intl
#RUN docker-php-ext-install pcntl
#RUN docker-php-ext-install pdo_mysql
#RUN docker-php-ext-install mbstring

RUN rm -rf /var/cache/apk/*
 
CMD ["php-fpm"]