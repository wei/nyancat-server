# Nyancat Telnet Server

[![Docker Stars](https://img.shields.io/docker/stars/ddhhz/nyancat-server.svg)](https://hub.docker.com/r/ddhhz/nyancat-server/) [![Docker Pulls](https://img.shields.io/docker/pulls/ddhhz/nyancat-server.svg)](https://hub.docker.com/r/ddhhz/nyancat-server/) [![Docker Build](https://img.shields.io/docker/build/ddhhz/nyancat-server.svg)](https://hub.docker.com/r/ddhhz/nyancat-server/builds/) [![ImageLayers Size](https://img.shields.io/imagelayers/image-size/ddhhz/nyancat-server/latest.svg)](http://imagelayers.io/?images=ddhhz/nyancat-server:latest) [![ImageLayers Layers](https://img.shields.io/imagelayers/layers/ddhhz/nyancat-server/latest.svg)](http://imagelayers.io/?images=ddhhz/nyancat-server:latest)

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
Wei He <docker@weispot.com>
