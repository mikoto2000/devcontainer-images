FROM mcr.microsoft.com/devcontainers/base:ubuntu-24.04

LABEL maintainer="mikoto2000 <mikoto2000@gmail.com>"
LABEL version="1.0.0"
LABEL description="vim-devkit"

COPY ./ubuntu.sources /etc/apt/sources.list.d/ubuntu.sources

RUN apt update \
    && apt build-dep -y vim \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

