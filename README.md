# docker-corretto-debian


A simple Dockerfile to build an image of Amazon Corretto based on Debian Linux.

## Pull a pre-built image

Check out the [Docker Repository](https://hub.docker.com/r/jogo81/corretto-debian)


## Build the image yourself

Building is straightforward:

```
docker build .
```

### Build Arguments
* `CORRETTO_VERSION`: Select the Java version

E.g., to build an image for Corretto 11 or 1.8:

```
docker build --build-arg CORRETTO_VERSION=11 .

docker build --build-arg CORRETTO_VERSION=1.8.0 .
```
