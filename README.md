# Nyancat Telnet Server

[![Docker Stars](https://img.shields.io/docker/stars/ddhhz/nyancat-server.svg)](https://hub.docker.com/r/ddhhz/nyancat-server/) [![Docker Pulls](https://img.shields.io/docker/pulls/ddhhz/nyancat-server.svg)](https://hub.docker.com/r/ddhhz/nyancat-server/) [![Docker Build](https://img.shields.io/docker/build/ddhhz/nyancat-server.svg)](https://hub.docker.com/r/ddhhz/nyancat-server/builds/) [![Docker Image Size and Layers](https://images.microbadger.com/badges/image/ddhhz/nyancat-server.svg)](https://microbadger.com/images/ddhhz/nyancat-server)

Docker Image for a nyancat telnet server.


## Usage

### Telnet Server
```bash
$ docker run -d --name nyancat-server --restart=always -p 23:23 ddhhz/nyancat-server
```

##### To view:
```bash
$ telnet <localhost or serverhost>
```

### View Locally, aka show me the cat
```bash
$ docker run -d --name nyancat-local ddhhz/nyancat-server

$ docker exec -it nyancat-local nyancat
```


## Using

### [klange/nyancat](https://github.com/klange/nyancat)
Checkout 「[Nyan Cat Telnet Server](http://nyancat.dakko.us/)」 project homepage for demos.

### [atsampson/onenetd](https://github.com/atsampson/onenetd)
> By default, 40 connections are allowed at once.

View `onenetd` help document by running `$ docker exec nyancat-server sh -c "onenetd -h"`


## Author
[**Wei He**](https://whe.me)  [_&#103;&#105;&#116;&#104;&#117;&#098;&#064;&#119;&#101;&#105;&#115;&#112;&#111;&#116;&#046;&#099;&#111;&#109;_](mailto:&#103;&#105;&#116;&#104;&#117;&#098;&#064;&#119;&#101;&#105;&#115;&#112;&#111;&#116;&#046;&#099;&#111;&#109;)
