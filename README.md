# Node

Docker image to run Node. Defaults to 6.9.1 (LTS) using the $NODE_VERSION env variable.

Installs some common system dependencies for NPM packages.

Use this a base image for Node applications or Front-End Development.

## Usage

The image builds Node using an ONBUILD command so the actual install of Node is deferred until you build another image using this image as the base.

### Use this image from Docker Hub

In your Dockerfile reference the prebuilt image as the base

		FROM lookitsatravis/node:6.9.1

### To build the image

		$ git clone https://github.com/lookitsatravis/docker-node.git
		$ cd docker-node
		$ docker build -t node:6.9.1 .

## License

MIT
