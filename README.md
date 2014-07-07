## Twisted Dockerfile

This repository contains a **Dockerfile** for [Twisted](https://www.twistedmatrix.com.com/), to be used to publish [trusted builds](https://index.docker.io/u/twisteds/twisted/) to the [Docker Registry](https://index.docker.io/).

The image is based on the official [Ubuntu 14.04 image](https://registry.hub.docker.com/_/ubuntu/).

This image is meant to be used as a base for any [Twisted](https://www.twistedmatrix.com.com/)-based applications.  It also includes all dependencies necessary for client and server TLS support.

### Installation

1. Install [Docker](https://www.docker.io/).
2. Download the [twisted trusted build](https://index.docker.io/u/twisted/baseimage/) from the [Docker Registry](https://index.docker.io/): `docker pull twisted/baseimage`

    You can also build the image yourself from the Dockerfile: `docker build -t="twisted/baseimage" github.com/twisted/baseimage`)

### Usage

In your `Dockerfile`, include the following line:

        FROM twisted/baseimage

Alternately, you can just run the image to test it:

    docker run -it --rm twisted/baseimage

### Changelog
- 2014-070-06 - initial build
