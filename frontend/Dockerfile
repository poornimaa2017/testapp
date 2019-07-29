#Basic Docker Image program
FROM centos:7
MAINTAINER poornimaa2017@gmail.com
RUN yum -y update
RUN yum -y install httpd
RUN mkdir /apps
WORKDIR /apps
#Extracts zip and copies the file, add will get files from url as well
ADD code /var/www/html
ENV BACKENDLB=test
EXPOSE 80
CMD ["apachectl","-D","FOREGROUND"]
