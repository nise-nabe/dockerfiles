Dockerfiles 
===========

## Preparation

Make own debian image.

```
$ curl -O https://raw.github.com/dotcloud/docker-debian/master/contrib/mkimage-debian.sh
$ sudo bash mkdimage-debian.sh nise_nabe/debian
$ sudo docker images
REPOSITORY             TAG                 IMAGE ID            CREATED             SIZE
(none)                 latest              aaaaaaaaaaaa        a minute ago        157.3 MB (virtual 157.3 MB)
$ sudo docker tag aaaaaaaaaaaa nise_nabe/debian
$ sudo docker tag aaaaaaaaaaaa nise_nabe/debian:wheezy
$ sudo docker images
REPOSITORY             TAG                 IMAGE ID            CREATED             SIZE
nise_nabe/debian        latest              aaaaaaaaaaaa        a minute ago        157.3 MB (virtual 157.3 MB)
nise_nabe/debian        wheezy              aaaaaaaaaaaa        a minute ago        157.3 MB (virtual 157.3 MB)
```

```
$ sudo docker build -t nise_nabe/base-chef -rm base-chef
```
