docker-builder
==============

The project aims to be an alternative to hosted docker.io image builder service.

Why
===

Docker.io offers a very useful service: not only it can host your public or private images, it also has a service that can be triggered by a GitHub or Bitbucket hook and create a build of the docker image.

The problem of this service is that is assumes the user wants to host the image on docker.io and it's not possible to tell him to push to another docker registry.
