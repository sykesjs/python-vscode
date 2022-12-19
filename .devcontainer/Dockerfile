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

# Install other python libraries
RUN pip3 install email-validator PyGithub microsoftgraph-python

# Install Powershell
# Download the Microsoft repository GPG keys
wget -q "https://packages.microsoft.com/config/ubuntu/22.10/packages-microsoft-prod.deb"

# Register the Microsoft repository GPG keys
sudo dpkg -i packages-microsoft-prod.deb

# Update the list of packages after we added packages.microsoft.com
sudo apt-get update

# Install PowerShell
sudo apt-get install -y powershell
