# Docker
## Intro

Docker is an open platform for developing, shipping, and running applications. 

Docker provides the ability to package and run an application in a container.

## Docker Engine

Docker Engine acts as a client-server application for building containers that can be accessed from the Terminal. 

It has the following components:

- A server with a long-running daemon process `dockerd`.
- APIs which specify interfaces that programs can use to talk to and instruct the Docker daemon.
- A command line interface (CLI) client `docker`.

## Docker Desktop

Docker Desktop is an easy-to-install application with a Graphical User Interface (GUI). 
It includes the Docker Engine and an easy to use GUI.
It is available for MacOS, Windows and Linux (deb package for Debian/Ubuntu and rpm package for Fedora/Red Hat).

## Docker Playground

You can also use [Play with Docker](https://labs.play-with-docker.com/) to learn Docker in an online environment.

## Docker Images
An image is a read-only template with instructions for creating a Docker container.

It usually consists of a file system with files and packages necessary to run your applications.

Often, an image is based on another image, with some additional customization. 

For example, you can start with the Python3 image, then install Flask, Flask-SQLAlchemy and other requirements and copy your source code files to create an image for your application.

From there you are able to create containers from your image. A container is a runnable instance of an image. 

A container is defined by its image as well as any configuration options you provide to it when you create or start it.

## Installation

Links to install Docker Desktop and Docker Engine can be found at: [Docker Installation Links](https://docs.docker.com/engine/install/)

You can install Docker Engine on Linux using the instructions at the following links:

- [Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
- [Fedora](https://docs.docker.com/engine/install/fedora/)
- [CentOS](https://docs.docker.com/engine/install/centos/)

## Test
```bash
touch Dockerfile
vim Dockerfile
[Alt + Enter]
```

Dockerfile
```docker
FROM alpine
CMD ["echo", "Testing Docker!!"]
```

```bash
[:wq + Enter]
cat Deockerfile
```
Build the image, create and run the container from the image:

```bash
docker build -t test .
docker image ls 
docker run --rm test
docker image rm test
```

## Docker Hub

Docker Hub is a service provided by Docker for finding and sharing container images. 

It is the world’s largest repository of container images.

You can create public repositories for free or choose a subscription plan for private repositories.

## Docker Hub Features

Docker Hub provides the following major features:

Repositories: Push and pull container images.
Teams & Organizations: Manage access to private repositories of container images.
Docker Official Images: Pull and use high-quality container images provided by Docker.
Docker Verified Publisher Images: Pull and use high- quality container images provided by external vendors.
Builds: Automatically build container images from GitHub and Bitbucket and push them to Docker Hub.
Webhooks: Trigger actions after a successful push to a repository to integrate Docker Hub with other services.

## Resources

- [Docker Documentation](https://docs.docker.com/get-started/overview/)
- [Docker Engine](https://docs.docker.com/engine/)
- [Docker Desktop](https://docs.docker.com/desktop/)
- [Docker Playground](https://labs.play-with-docker.com/)
- [Docker Hub - Python](https://hub.docker.com/_/python)
- [Docker Command Reference - image](https://docs.docker.com/engine/reference/commandline/image/)
- [Docker Command Reference - container](https://docs.docker.com/engine/reference/commandline/container/)
- [Docker Hub](https://docs.docker.com/docker-hub/)

