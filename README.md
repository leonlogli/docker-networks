# Docker "Docker networks" Example

Docker example that shows how networks work.

## Prerequisites

Before you get started, you need to have the following tools installed:

- Docker

## Running the "Docker networks" Container

Navigate to the root directory of the cloned repository:

Build the Docker image:

```bash
docker build -t docker-networks .
```

Create docker network:

```bash
docker network create docker-networks
```

Run mongo db container in the created network `docker-networks`:

```bash
docker run -d --name docker-networks-db --network docker-networks mongo
```

Run the Docker container in the same network:

```bash
docker run -d -p 8080:3000 --rm --network multi-containers --name docker-networks docker-networks
```
