# danirus/django-comments-xtd-demo:2.0.5

`Dockerfile` to create a [Docker](https://www.docker.com/) container image to test the django-comments-xtd demo project.

The Django demo project provides comments support to several models, defining the maximum thread level on per app.model basis. The demo expose multiple features like moderation, removal suggestion flags, like/dislike flags, and list of users who liked/disliked comments. 

Users can send comments to Articles and Quotes. Comments for Articles are handled through the ReactJS plugin included with django-comments-xtd while comments for Quotes use no JavaScript.

## Installation

Automated builds of the image are available on [Dockerhub](https://hub.docker.com/r/danirus/django-comments-xtd-demo) and is the recommended method of installation.

```bash
docker pull danirus/django-comments-xtd:2.0.5
```

Alternatively you can build the image yourself.

```bash
docker build -t danirus/django-comments-xtd-demo github.com/danirus/docker-django-comments-xtd-demo
```

## Quickstart

Start the demo project using:

```bash
docker run -d --name django-comments-xtd-demo --restart=always --publish 80:8000 danirus/django-comments-xtd-demo:2.0.5
```
