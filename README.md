## Twisted Dockerfile

This repository contains a **Dockerfile** for [Twisted](https://www.twistedmatrix.com.com/).

The image is based on the official [Ubuntu 14.04 image](https://registry.hub.docker.com/_/ubuntu/).

This image is meant to be used as a base for any [Twisted](https://www.twistedmatrix.com.com/)-based applications.  It also includes all dependencies necessary for client and server TLS support.

### Installation

1. Install [Docker](https://www.docker.io/).
2. `docker build -t="twisted/baseimage" github.com/cyli/docker-twisted`)

### Usage

In your `Dockerfile`, include the following line:

        FROM twisted/baseimage

Alternately, you can just run the image to test it:

    docker run -it --rm twisted/baseimage

### Changelog
- 2014-07-06 - initial build/commit
