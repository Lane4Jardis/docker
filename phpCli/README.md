# Lane4 Digital PHP CLI

![Build Status](https://github.com/lane4jardis/docker/actions/workflows/phpCli.yml/badge.svg)
[![Docker Image Version](https://img.shields.io/docker/v/lane4jardis/phpcli?sort=semver)](https://hub.docker.com/r/lane4jardis/phpcli)

### Providing Versioned PHP Docker Images for Console Applications

The **Lane4 PHP CLI** tool is designed to deliver cross-platform PHP-CLI Docker images. It supports PHP versions from **7.4 to 8.3**, enabling developers and administrators to create and maintain consistent and reliable environments for their console applications.

Our Docker images are available for both **AMD64** and **ARM64** architectures and are hosted on [Docker Hub](https://hub.docker.com/r/lane4jardis/phpcli). This ensures broad compatibility and allows deployment across various hardware platforms, including modern servers and IoT devices.

### The following components were applied:
- alpine 7.4 - 8.3 base image
- xdebug
- pdo
- mysql
- redis
- curl
- dom
- soap
- zip
- mbstring

### Image sizes
- Between 100MB and 107MB :-)

## Prerequisites

Please refer to the installation prerequisites outlined in the `README.md` located in the root directory of the Docker project repository.

## Usage

We have created a `Makefile` that provides all available usage options through the `make` command in the terminal.

## Customization for Your Needs

If you wish to fully customize the tool to meet your specific requirements, please edit the relevant entries in the `.env` file.

This allows for flexible configuration of the provided Docker images, including specific PHP extensions, configuration settings, and other customizations.

For this type of usage, you will need your own source and image repository.

We would greatly appreciate it if you could acknowledge us as a supporter of your Docker images in such cases.

## Contents of `phpCli`

The `phpCli` package includes the following components:

- **Source Files**:
    - `/phpcli` – Contains the source code and configuration files for the PHP-CLI tool.

- **Support Files**:
    - `.env` – Environment variables for configuring the Docker images.
    - `docker-compose.yml` – Docker Compose configuration file for orchestrating the containers.
    - `Dockerfile` – Dockerfile for building the PHP-CLI images.
    - `Makefile` – Simple command-line helper. Run `make` in the terminal to view available commands.
    - `.github/workflows/phpCli.yml` – GitHub Actions workflow for automating builds and tests.

- **Documentation**:
    - `README.md` – Comprehensive documentation and guides for using the tool.
