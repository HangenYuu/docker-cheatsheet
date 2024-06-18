# Markdown version of the official Docker cheatsheet
> The official cheatsheet can be found [here](https://docs.docker.com/get-started/docker_cheatsheet.pdf).

This is the Markdown version of the official Docker cheatsheet, optimized for copy and paste! All rights belong to Docker.

# Installation
- Docker Desktop is the official and easiest way to install a bundle of Docker Engine and other useful components: https://docs.docker.com/desktop/install
- Docker Engine can be installed separate if you are using a VM without a GUI: https://docs.docker.com/engine/install
- Docker Compose plugin can be installed separately after Docker Engine and Docker CLI: https://docs.docker.com/compose/install
- VS Code Docker extension for a GUI to work with Docker images, containers and more: https://code.visualstudio.com/docs/containers/overview
- General documentation: https://docs.docker.com/

# Images CLI 
Docker images are a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

- Build an Image from a Dockerfile
```bash
docker build -t <image_name>
```
- Build an Image from a Dockerfile without the cache
```bash
docker build -t <image_name> . --no-cache
```
- List local images
```bash
docker images
```
- Delete an Image
```bash
docker rmi <image_name>
```
- Remove all unused images
```bash
docker image prune
```