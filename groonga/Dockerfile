FROM debian:wheezy
MAINTAINER nise_nabe <nise.nabe@gmail.com>

RUN echo "deb http://packages.groonga.org/debian/ wheezy main\ndeb-src http://packages.groonga.org/debian/ wheezy main" >> /etc/apt/sources.list.d/groonga.list
RUN apt-get update
RUN apt-get -y --allow-unauthenticated install groonga-keyring
RUN apt-get update
RUN apt-get -y install groonga groonga-tokenizer-mecab
