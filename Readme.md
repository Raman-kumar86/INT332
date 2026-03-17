# Daily Study Notes - Docker Fundamentals

## DockerHub (Centralized Registry for Docker Images)
DockerHub is a cloud-based repository where Docker images are stored, managed, and shared.
It helps teams distribute application images consistently and pull ready-to-use images quickly.

## Docker Architecture
Docker follows a client-server architecture where commands are sent by the client and processed by the Docker Engine.
This architecture makes container creation, image management, and deployment efficient across local and remote systems.

## Key Components

### Docker Client
The Docker Client is the command-line interface (`docker` command) used by users to interact with Docker.
It sends requests such as build, run, and pull to the Docker Daemon.

### Docker Daemon
Docker Daemon (`dockerd`) is the background service that builds, runs, and manages containers and images.
It listens for Docker API requests and performs the actual container operations.

### Docker Images
Docker Images are read-only templates used to create containers.
They include application code, dependencies, and configuration needed to run an application.

### Containers
Containers are running instances of Docker images.
They are lightweight, isolated environments that package an application with everything it needs to execute.

### Docker Registry (DockerHub)
A Docker Registry stores Docker images, and DockerHub is the most widely used public registry.
You can push your own images to it and pull images created by others.

## Docker Life Cycle
Docker workflow generally follows three stages: Build, Ship, and Run.
In Build, you create images; in Ship, you push/pull images through registries; in Run, you start containers from those images.

## Container States

### Created
The container is created but not started yet.
This state appears after container setup is complete and before execution begins.

### Running
The container is actively executing its main process.
In this state, the application inside the container is live and available for use.
