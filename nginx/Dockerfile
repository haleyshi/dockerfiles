# version 0.0.1
FROM ubuntu:14.04
MAINTAINER Shi Guohuang "sgh1982@gmail.com"
ENV REFRESHED_AT 2017-11-23
RUN apt-get -qq update
RUN apt-get install -y nginx
#RUN echo 'Hi. I am in your container' > /usr/share/nginx/html/index.html
ADD html.tar.gz /usr/share/nginx/
EXPOSE 80
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
