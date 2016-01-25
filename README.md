# Docker containers

These docker containers are adaptations of the [rocker](https://github.com/rocker-org/rocker) and [hadley](https://github.com/hadley/docker) containers.

## To build

```sh
cd /package/dir

docker pull rocker/r-devel # ensure we have latest devel image
docker build -t bobbyloco/r-devel .
```

## To use

```sh
cd /package/dir

docker run --rm -it bobbyloco/r-devel bash
```
