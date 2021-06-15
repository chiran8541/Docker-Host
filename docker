FROM centos:latest
MAINTAINER Chiran
RUN yum install httpd\zip \ unzip
ADD https://www.free-css.com/assets/files/free-css-templates/download/page268/rento.zip /var/www/html/
WORKDIR /var/www/html
RUN unzip rento.zip
RUN cp -rvf markups-rento/* .
RUN rm -rf __MACOSX markups-rento rento.zip
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]
EXPOSE 80
