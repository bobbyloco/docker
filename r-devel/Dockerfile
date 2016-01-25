## Adapted from rocker/r-devel and hadley/docker
FROM rocker/r-devel:latest

# Packages needed for full R CMD check
RUN apt-get update -qq && apt-get install -t unstable -y --no-install-recommends \
    aspell \
    aspell-en \
    ghostscript \
    imagemagick \
    lmodern

# Common dev headers
RUN apt-get update -qq && apt-get install -t unstable -y --no-install-recommends \
    libcairo2-dev \
    libmysqlclient-dev \
    libpq-dev \
    libssl-dev \
    libsqlite3-dev \
    libxml2-dev

# Install devtools and testthat
RUN Rscript -e 'install.packages(c("devtools","testthat"),dependencies = TRUE)'
