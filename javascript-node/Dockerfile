FROM mcr.microsoft.com/devcontainers/base:ubuntu-24.04

# common info
ARG NODE_VERSION=v22.13.1
ENV PATH=$PATH:/opt/node-${NODE_VERSION}-linux-x64/bin

# Install npm
RUN curl -LO https://nodejs.org/dist/${NODE_VERSION}/node-${NODE_VERSION}-linux-x64.tar.xz \
    && tar xf ./node-${NODE_VERSION}-linux-x64.tar.xz -C /opt \
    && rm ./node-${NODE_VERSION}-linux-x64.tar.xz

ARG USERNAME=vscode

