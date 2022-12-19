FROM ubuntu:kinetic-20221101

LABEL maintainer="BurnsMcD Platform Engineering"
LABEL description="Container for Python Scripting"

# Install Dependencies
RUN apt-get update

RUN apt-get install sudo \
    git \
    bash \
    curl \
    wget \
    apt-transport-https \
    software-properties-common \
    gpg \
    unzip \
    tar \
    python3-pip \
    nano \
    gettext-base \
    jq \
    -y

# Use /tmp for installs
WORKDIR /tmp

# Install pre-commit hook support
RUN pip3 install pre-commit
