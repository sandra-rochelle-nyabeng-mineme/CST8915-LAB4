# Lab 4 - CST8915 Full-stack Cloud-native Development: Introduction to Docker
### Sandra Rochelle Nyabeng Mineme -- 041268641

### : youtube link :https://youtu.be/2Vphe1NlIn0

## Reflection Questions

## What are the main differences between a Docker image and a Docker container?

A docker image is a blueprint. It contains the code, libraries and dependencies needed to run application. A docker container is a running instance of that image.

The docker image is like a recipe and the container is the actual dish created from it.
## Explain how Docker's layered architecture improves efficiency.

Each layer of docker images represent a change. This layered system allows Docker to reuse layers across different images, so if multiple images share the same base, those layers don't need to be rebuilt or re-downloaded.

This reduce build time, storage use, and bandwidth consumption.

## Why does each container get its own writable layer?

It can modify files and create new data independently without affecting the original image or other containers.
It can run from the same image while maintaining isolated runtime states.

## What are the benefits of using Docker Compose over running containers individually?

Docker compose simplifies managing multi-container applications. Instead of running multiple docker run commands, with one command docker compose up, compose brings up the entire stack, making it to develop, scale and maintain consistent environments.