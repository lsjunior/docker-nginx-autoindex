docker-nginx-autoindex
======================

Dockerfile for Nginx with autoindex, **WITHOUT IPV6!**

[![CI to Docker Hub](https://github.com/dceoy/docker-nginx-autoindex/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/dceoy/docker-nginx-autoindex/actions/workflows/docker-publish.yml)

Docker image
------------

Pull the image from [Docker Hub](https://hub.docker.com/r/lsjunior/nginx-autoindex/)

```sh
$ docker image pull dceoy/nginx-autoindex
```

Usage
-----

Run a web server to serve the current directory at `/` of Nginx

```sh
$ docker container run --rm -p 80:80 -v ${PWD}:/var/lib/nginx/html:ro lsjunior/nginx-autoindex
```

Run a web server with docker-compose

```sh
$ docker-compose -f /path/to/docker-nginx-autoindex/docker-compose.yml up
```
