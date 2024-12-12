# Docker Repository

Welcome to the Docker repository! This repository contains basic Docker examples and guides to help you get started with containerization and running lightweight applications.

## Table of Contents

- [Overview](#overview)
- [Getting Started](#getting-started)
- [Basic Commands](#basic-commands)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Overview

This repository serves as an introduction to Docker, providing simple examples for creating and managing containers. It is suitable for beginners looking to understand how Docker works.

## Getting Started

To begin using Docker with this repository:

1. Install Docker on your machine. Follow the [Docker installation guide](https://docs.docker.com/get-docker/).
2. Clone this repository:

   ```bash
   git clone git@github.com:kumsa-Mergia/Docker.git
   cd docker-repository
   ```
3. Explore the example Dockerfiles and use them to build and run containers.

## Basic Commands

Here are some essential Docker commands to get you started:

- **Check Docker version:**
  ```bash
  docker --version
  ```

- **List all Docker images:**
  ```bash
  docker images
  ```

- **Run a simple container (e.g., an Ubuntu shell):**
  ```bash
  docker run -it ubuntu /bin/bash
  ```

- **List running containers:**
  ```bash
  docker ps
  ```

- **Stop a container:**
  ```bash
  docker stop container-id
  ```

- **Remove a container:**
  ```bash
  docker rm container-id
  ```

## Examples

This repository includes basic Docker examples such as:

- A simple Nginx web server:
  ```bash
  docker run -d -p 8080:80 nginx
  ```

- Building a custom image using a provided Dockerfile:
  ```bash
  docker build -t custom-image-name ./examples/basic-example
  ```

- Running a containerized Python application:
  ```bash
  docker run -it python:3.8 python
  ```

