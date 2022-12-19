# Visual Studio Code Python Environment

This repository includes tools for doing containerized development for Python 3.

## Local Setup

### Install Visual Studio Code 

Download and install Visual Studio Code. 

On Mac's with homebrew:

```  brew install --cask visual-studio-code ```

On a PC with chocolatey

``` choco install vscode ```

Alternatively, [manually download](https://code.visualstudio.com/download) and install on your local workstation.

### Install a container runtime environment

Install the container runtime of your choice. For example [Docker Desktop](https://www.docker.com/products/docker-desktop/).

### Install Visual Studio Code Extensions

1. Install [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
2. (Optional) Install the [Docker Extension](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)

## Fork and Clone the Repository

Fork this repository.
Clone the forked repository and open the local checkout in Visual Studio Code.
When prompted, click "Open in Container."
This will cause the build of the container.
The terminal should open inside the continer with the repository monted.