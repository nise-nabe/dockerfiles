FROM nise_nabe/debian:wheezy
MAINTAINER nise_nabe <nise.nabe@gmail.com>

RUN apt-get update
RUN apt-get --yes install curl

RUN curl -L https://www.opscode.com/chef/install.sh | bash
RUN echo 'export PATH=${PATH}:/opt/chef/embedded/bin' >> /etc/bash.bashrc
RUN /opt/chef/embedded/bin/gem install knife-solo --no-ri --no-rdoc
