FROM nise_nabe/base-chef
MAINTAINER nise_nabe <nise.nabe@gmail.com>

RUN apt-get update

ADD chef-repo /opt/nise_nabe/chef-repo
ADD solo.rb /opt/nise_nabe/chef-repo/solo.rb

RUN chef-solo -c /opt/nise_nabe/chef-repo/solo.rb -j /opt/nise_nabe/chef-repo/nodes/base.json
