# Root Repository for Single-SPA Project

This repository serves as the root configuration for a Single-SPA project that includes multiple micro-frontends. It contains a `docker-compose.yml` file to manage the Docker containers for the root configuration and the various micro-frontends.

## Repository Structure

- **Docker Configuration**: `docker-compose.yml` file for setting up and running the project in Docker containers.
- **Git Submodules**: Includes references to the root-config and other micro-frontends as Git submodules.

## Getting Started

### Prerequisites

Ensure you have Docker and Docker Compose installed on your machine.

- [Docker Installation](https://docs.docker.com/get-docker/)
- [Docker Compose Installation](https://docs.docker.com/compose/install/)

### Cloning the Repository

Clone the repository including its submodules:

```bash
git clone --recurse-submodules https://github.com/isoftchamp/microfront-main.git
cd your-root-repo
```

### Docker Setup

To build and start the Docker containers, use the following commands:

#### 1. Build the Docker containers:

```bash
docker compose build
```

#### 2. Start the Docker containers:

```bash
docker compose up
```

This will start all the services defined in docker-compose.yml, including the root configuration and micro-frontends.

## Submodules
This repository includes the following Git submodules:

* Root Config: root-config
* React Micro-Frontend: react-app

To initialize and update the submodules, run:
```bash
git submodule update --init --recursive
```

## Project Structure
* `docker-compose.yaml`: Defines and configures Docker services.
* `.gitmodules`: Lists the submodules included in this repository.
* `root-config`: Directory for the root configuration.
* `react-app`: Directory for the react micro-frontend.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
