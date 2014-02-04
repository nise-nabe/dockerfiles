FROM debian:wheezy
MAINTAINER nise_nabe <nise.nabe@gmail.com>

RUN export LC_ALL=C

RUN apt-get update && apt-get upgrade -y && apt-get clean
RUN apt-get --yes install curl git locales locales-all
RUN apt-get install -y openssh-server --no-install-recommends
