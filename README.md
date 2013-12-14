Dockerfiles 
===========

## Preparation

Make own debian image.

```
$ curl -O https://raw.github.com/dotcloud/docker-debian/master/contrib/mkimage-debian.sh
$ sudo bash mkdimage-debian.sh nise-nabe/debian
$ sudo docker images
REPOSITORY             TAG                 IMAGE ID            CREATED             SIZE
(none)                 latest              aaaaaaaaaaaa        a minute ago        157.3 MB (virtual 157.3 MB)
$ sudo docker tag aaaaaaaaaaaa nise-nabe/debian
$ sudo docker tag aaaaaaaaaaaa nise-nabe/debian:wheezy
$ sudo docker images
REPOSITORY             TAG                 IMAGE ID            CREATED             SIZE
nise-nabe/debian        latest              aaaaaaaaaaaa        a minute ago        157.3 MB (virtual 157.3 MB)
nise-nabe/debian        wheezy              aaaaaaaaaaaa        a minute ago        157.3 MB (virtual 157.3 MB)
```
