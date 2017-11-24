# apache2
FROM ubuntu:12.04
MAINTAINER Shi Guohuang "sgh1982@gmail.com"
RUN apt-get -qq update
RUN apt-get install -y apache2
ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2
ONBUILD ADD . /var/www/
EXPOSE 80
ENTRYPOINT ["/usr/sbin/apache2", "-D", "FOREGROUND"]
#CMD ["/usr/sbin/apache2", "-D", "FOREGROUND"]
