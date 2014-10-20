docker-builder
==============

The project aims to be an alternative to hosted docker.io image builder service.

Why
===

Docker.io offers a very useful service: not only it can host your public or private images, it also has a service that can be triggered by a GitHub or Bitbucket hook and create a build of the docker image.

The problem of this service is that is assumes the user wants to host the image on docker.io and it's not possible to tell him to push to another docker registry.

What
====

The service will show a very basic dashboard (we could skip this at the beginning and just use some config file) to add a new build configuration and see the existing ones.

 * We connect to GitHub and setup permissions
 * We select: project, Dockerfile path, branch/tag, name, tag, push url, notify url (at this point an hook is setup on GitHub)
 * Service listen to connection from GitHub hooks
 * Pulls the latest code locally
 * Builds the image using Dockerfile
 * Push the image to the push url
 * Notifies the notify url
 * Send an email with build result

Contribute
==========

The project is still in early stage (basically not started yet) and the idea is to write it in Python. If anyone is willing to contribute, please get in touch with us.

Authors
=======

This project is being developed by:

 * Andrea Grandi (andreagrandi)
 * Christoph Witzany (DoubleMalt)
