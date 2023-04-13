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

Run the Docker container:

```bash
docker run -d -p 8080:3000 --rm --name docker-networks docker-networks
```
