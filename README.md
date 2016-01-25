# Docker containers

These docker containers are adaptations of the [rocker](https://github.com/rocker-org/rocker), [hadley](https://github.com/hadley/docker), and [cardcorp](https://github.com/cardcorp/card-rocker) containers.

## To build

```sh
cd /package/dir
docker build -t bobbyloco/R .
```

## To use

```sh
cd /package/dir
docker run --rm -it bobbyloco/R bash
```
