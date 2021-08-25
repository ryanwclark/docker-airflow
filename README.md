# github.com/ryanwclark/docker-airflow

[![GitHub release](https://img.shields.io/github/v/tag/ryanwclark/docker-airflow?style=flat-square)](https://github.com/ryanwclark/docker-airflow/releases/latest)
[![Build Status](https://img.shields.io/github/workflow/status/ryanwclark/docker-airflow/build?style=flat-square)](https://github.com/ryanwclark/docker-airflow/actions?query=workflow%3Abuild)
[![Docker Stars](https://img.shields.io/docker/stars/ryanwclark/airflow.svg?style=flat-square&logo=docker)](https://hub.docker.com/ryanwclark/airflow/)
[![Docker Pulls](https://img.shields.io/docker/pulls/ryanwclark/airflow.svg?style=flat-square&logo=docker)](https://hub.docker.com/ryanwclark/airflow/)


* * *


## About

Dockerfile to build an [airflow](https://airflow.apache.org/) container image.

* Currently tracking 2.1.0

## Maintainer

- [Ryan Clark](https://github.com/ryanwclark)

## Table of Contents

- [About](#about)
- [Maintainer](#maintainer)
- [Table of Contents](#table-of-contents)
- [Prerequisites and Assumptions](#prerequisites-and-assumptions)
- [Installation](#installation)
- [Configuration](#configuration)
  - [Quick Start](#quick-start)
  - [Persistent Storage](#persistent-storage)
  - [Environment Variables](#environment-variables)
- [Debug Mode](#debug-mode)
- [Maintenance](#maintenance)
- [Support](#support)
- [License](#license)
- [References](#references)

## Prerequisites and Assumptions

No prerequisites required

## Installation

### Build from Source
Clone this repository and build the image with `docker build <arguments> (imagename) .`

### Prebuilt Images
Builds of the image are available on [Docker Hub](https://hub.docker.com/ryanwclark/airflow) and is the recommended method of installation.

```bash
docker pull ryanwclark/airflow:(imagetag)
```

The following image tags are available along with their tagged release based on what's written in the [Changelog](CHANGELOG.md):

| airflow version | Tag     |
| -------------- | ------- |
| `main`         | `:main` |


## Configuration

### Quick Start


### Persistent Storage

The following directories are used for configuration and can be mapped for persistent storage.

| Directory                           | Description                          |
| ----------------------------------- | ------------------------------------ |
| `/dags`                             | It's your dag bag                    |


### Environment Variables



## Maintenance

### Shell Access


## Support

These images were built to serve a specific need in a production environment and gradually have had more functionality added based on requests from the community.
### Usage
- The [Discussions board](../../discussions) is a great place for working with the community on tips and tricks of using this image.

### Bugfixes
- Please, submit a [Bug Report](issues/new) if something isn't working as expected. I'll do my best to issue a fix in short order.

### Feature Requests
- Feel free to submit a feature request, however there is no guarantee that it will be added, or at what timeline.


### Updates
- Best effort to track upstream changes, More priority if I am actively using the image in a production environment.


## License
MIT. See [LICENSE](LICENSE) for more details.
