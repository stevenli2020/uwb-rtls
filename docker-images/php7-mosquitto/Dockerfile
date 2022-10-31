FROM php:7.4-apache
MAINTAINER steven <steven@gmail.com> 

RUN apt-get update 
RUN apt-get install -y sudo wget curl net-tools nano libmosquitto-dev
RUN apt-get clean
RUN pecl install Mosquitto-alpha
RUN echo "extension=mosquitto.so" > /usr/local/etc/php/conf.d/mosquitto.ini
RUN a2enmod rewrite
EXPOSE 80


