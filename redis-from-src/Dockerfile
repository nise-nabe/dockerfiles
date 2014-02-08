FROM debian:wheezy
MAINTAINER nise_nabe <nise.nabe@gmail.com>

RUN apt-get -qq update && apt-get --yes upgrade
RUN apt-get --yes install curl git-core

RUN apt-get --yes install build-essential python

RUN cd /usr/local/src \
  && curl -O http://download.redis.io/redis-stable.tar.gz \
  && tar xvzf redis-stable.tar.gz \
  && cd redis-stable \
  && make \
  && make install

EXPOSE 6379
CMD redis-server
