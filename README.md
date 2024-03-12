# Drupal Docker Development Environment

This repository provides a Docker-based development environment for Drupal using Docker Compose.

## Prerequisites

Before using this Docker setup, ensure you have the following installed:

- Docker Engine
- Docker Compose

## Getting Started

To set up a local Drupal development environment using Docker:

1. Clone this repository:


```bash
git clone https://github.com/kahnu044/drupal-docker-with-postgres
```


2. Navigate to the repository directory:

```bash
cd drupal-docker-with-postgres
```

3. Start the Docker containers using Docker Compose:

```bash
docker-compose up -d
```

4. Access Drupal in your web browser at http://localhost:8019. Follow the Drupal installation instructions.

## Services

This Docker Compose setup includes the following services:

- **Drupal**: The latest version of Drupal running on Apache, accessible at http://localhost:8019.
- **PostgreSQL**: The latest version of PostgreSQL as the database backend for Drupal.

## Configuration

- The Drupal files (modules, themes, profiles) are mounted from the `./drupal` directory into the Drupal container.
- The PostgreSQL data is stored in the `./data/db` directory on the host machine.

## Customization

You can customize this Docker setup by modifying the `docker-compose.yml` file and adding additional Docker-related configuration files as needed.

## Author

[Kahnu Charan Swain](https://github.com/kahnu044)
