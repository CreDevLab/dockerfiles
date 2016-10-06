FROM ubuntu

MAINTAINER Credevlabz <docker@credevlabz.org>

RUN apt-get update 
RUN apt-get install nginx -y
#RUN netstat -plntu | grep 80
RUN apt-get install php7.0-fpm php7.0-mcrypt php7.0-curl php7.0-cli php7.0-mysql php7.0-gd php7.0-xsl php7.0-json php7.0-intl php-pear php7.0-dev php7.0-common php7.0-mbstring php7.0-zip php-soap libcurl3 curl -y
RUN systemctl restart php7.0-fpm
RUN cd ~/
RUN curl -sS https://getcomposer.org/installer | php && mv composer.phar /usr/bin/composer
WORKDIR /var/www/html

EXPOSE 80 443
