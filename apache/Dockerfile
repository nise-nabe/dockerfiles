FROM debian
MAINTAINER nise_nabe <nise.nabe@gmail.com>

RUN apt-get update && apt-get -y upgrade  && apt-get clean
RUN apt-get install -y apache2

ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2
CMD /usr/sbin/apache2 -D FOREGROUND
