# Docker containers

> This is my docker container. There are many like it, but this one is mine.
> 
> My container is my best friend. It is my life. I must master it as I must 
> master my life.

These docker containers are adaptations of the [rocker](https://github.com/rocker-org) and [hadley](https://github.com/hadley/docker) containers.

## To build

```sh
docker pull rocker/r-devel # ensure we have latest devel image
docker build -t bobbyloco/r-devel .
```

## To use

```sh
cd /package/dir

docker run --rm -it bobbyloco/r-devel bash
```
