# Docker
## Intro

Docker is an open platform for developing, shipping, and running applications. 

Docker provides the ability to package and run an application in a container.

Docker Engine is a terminal 

Docker Desktop is an easy-to-install application for your Mac or Windows environment that enables you to build and share containerized applications and microservices. It is available for MacOS, Windows and Linux (deb package for Debian/Ubuntu and rpm package for Fedora/Red Hat).

You can also use [Play with Docker](https://labs.play-with-docker.com/) to learn Docker in an online environment.

Docker Engine

## Docker Images
An image is a read-only template with instructions for creating a Docker container.

It usually consists of a file system with files and packages necessary to run your applications.

Often, an image is based on another image, with some additional customization. 

For example, you can start with the Python3 image, then install Flask, Flask-SQLAlchemy and other requirements and copy your source code files to create an image for your application.

From there you are able to create containers from your image. A container is a runnable instance of an image. 

A container is defined by its image as well as any configuration options you provide to it when you create or start it.

## Test
Dockerfile
```docker
FROM alpine
CMD ["echo", "Running Container!!"]
```
```bash
docker build -t hello .
docker build -t hello .
```
## Resources

https://docs.docker.com/get-started/overview/

https://docs.docker.com/get-docker/
