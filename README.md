# Super Chainsaw

__Super Chainsaw goes VROOM__

This repository represents an extremely basic containerized web application backend. It goes VROOM.

The application runs on port 8080.

## Purpose

The purpose of this repository is to represent a simple but 'real' application for exploration of Docker and Kubernetes.

## Prerequisites

- Node v16
- Docker Desktop

## Usage

1. Run `npm install` to install necessary packages.
2. Run `npm start` to run the server on port 8080.

## Building the Image

To build the Docker image run

```
docker build . -t <your username>/super-chainsaw:<tag>
```

## Running the Docker Image

Once you have built a docker image you can run it with

```
docker run -p 49160:8080 <your username>/super-chainsaw:<tag>
```

The application is now accessible at http://0.0.0.0:49160

## Shutting down the Docker Image

Get the Container ID

```
docker ps
```

Shut down the image

```
docker kill <container id>
```

## Recommended Utilities

- [avn](https://github.com/wbyoung/avn) - Automatic Version Switching for Node.js

## Notable Docs

[Node.js Docker Best Practices](https://github.com/nodejs/docker-node/blob/main/docs/BestPractices.md)