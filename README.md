# Nyancat Telnet Server

[![Docker Stars](https://img.shields.io/docker/stars/ddhhz/nyancat-server.svg)](https://hub.docker.com/r/ddhhz/nyancat-server/)
[![Docker Pulls](https://img.shields.io/docker/pulls/ddhhz/nyancat-server.svg)](https://hub.docker.com/r/ddhhz/nyancat-server/)
[![Docker Build](https://img.shields.io/docker/build/ddhhz/nyancat-server.svg)](https://hub.docker.com/r/ddhhz/nyancat-server/builds/)
[![ImageLayers Size](https://img.shields.io/imagelayers/image-size/ddhhz/nyancat-server/latest.svg)](http://imagelayers.io/?images=ddhhz/nyancat-server:latest)
[![ImageLayers Layers](https://img.shields.io/imagelayers/layers/ddhhz/nyancat-server/latest.svg)](http://imagelayers.io/?images=ddhhz/nyancat-server:latest)

Docker Image for a nyancat telnet server.


## Usage

### Telnet Server
```bash
$ docker run -d --name nyancat-server --restart=always -p 23:23 ddhhz/nyancat-server
```

To view:
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
Checkout 「[Nyan Cat Telnet Server](http://nyancat.dakko.us/)」 homepage for demos.

### [atsampson/onenetd](https://github.com/atsampson/onenetd)
> By default, 40 connections are allowed at once.

<details>
  <summary>View help document by running `$ docker exec nyancat-server sh -c "onenetd -h"`.</summary>

```
onenetd version 12

Usage: onenetd [options] address port command ...
  address  Address to bind to (0 for all local addresses)
  port     TCP port to bind to (0 for any available port)
  command  Command to execute
Options:
  -c N     limit to at most N children running (default 40).
           Further connections will be deferred unless -r
           is specified.
  -6       bind to an IPv6 address (default IPv4)
  -g gid   setgid(gid) after binding
  -u uid   setuid(uid) after binding
  -U       setuid($UID) and setgid($GID) after binding
  -1       print local port number to stdout after binding
  -b N     set listen() backlog to N
  -D       set TCP_NODELAY option on sockets
  -e       redirect stderr of children to socket
  -v       be verbose
  -Q       don't be verbose (default)
  -r resp  once -c limit is reached, refuse clients
           with 'resp' rather than deferring them.
           resp may contain \r, \n, \t.
  -h       show this usage message

Report bugs to <ats@offog.org>.
```
</details>


## Author
Wei He <github@weispot.com>
