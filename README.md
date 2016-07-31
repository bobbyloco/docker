# Docker containers

These docker containers are adaptations of the [rocker](https://github.com/rocker-org/rocker), [hadley](https://github.com/hadley/docker), and [cardcorp](https://github.com/cardcorp/card-rocker) containers.

## Docker Containers ##
| Docker Container Source on GitHub               | Docker Hub Build Status and URL
| :---------------------------------------        | :-----------------------------------------
| r-devtools (base + pandoc + devtools)           | [good](https://registry.hub.docker.com/u/zamora/r-devtools/)
| r-dsci (devtools + dplyr, rstan, etc...)        | [good](https://registry.hub.docker.com/u/zamora/r-dsci/)

### r-devtools
Builds on cardcorp/r-pandoc and adds R packages `devtools` and `testthat` and linux libraries `libcurl`, `libssl`, `sqlite3`, `xml2`, `qpdf`, and `vim`.

### r-dsci
Builds on r-devtools and adds R packages `dplyr`, `ggplot2`, `rstan`, and `tidyr` 

## Example build
```sh
cd /package/dir
docker build -t bobbyloco/r-devtools .
```

## Example use
```sh
cd /package/dir
docker run --rm -it bobbyloco/r-devtools bash
```
