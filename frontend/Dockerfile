#Basic Docker Image program


FROM ubuntu:18.04
MAINTAINER poornimaa2017@gmail.com
RUN apt-get -y update
RUN apt-get -y install tzdata
ENV TZ=Asia/Kolkota
RUN apt-get -y install nginx php php-gd php-mysql

ADD code /var/www/html
EXPOSE 80
CMD ["nginx","-g","daemon off;"]

