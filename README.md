In order to unify the approaches followed for Bitnami containers and Bitnami Helm charts, we are moving the different `bitnami/bitnami-docker-<container>` repositories to a single monorepo `bitnami/containers`. Please follow [bitnami/containers](https://github.com/bitnami/containers) to keep you updated about the latest Bitnami images.

More information here: https://blog.bitnami.com/2022/07/new-source-of-truth-bitnami-containers.html
# RabbitMQ Default User Credential Updater

## What is RabbitMQ Default User Credential Updater?

> RabbitMQ Default User Credential Updater is a component of the RabbitMQ Cluster Operator Helm chart that enables Hashicorp Vault integration.

[Overview of RabbitMQ Default User Credential Updater](https://github.com/rabbitmq/default-user-credential-updater)

Trademarks: This software listing is packaged by Bitnami. The respective trademarks mentioned in the offering are owned by the respective companies, and use of them does not imply any affiliation or endorsement.

## TL;DR

```console
$ docker run --name rmq-default-credential-updater bitnami/rmq-default-credential-updater:latest
```

## Why use Bitnami Images?

- Bitnami closely tracks upstream source changes and promptly publishes new versions of this image using our automated systems.
- With Bitnami images the latest bug fixes and features are available as soon as possible.
- Bitnami containers, virtual machines and cloud images use the same components and configuration approach - making it easy to switch between formats based on your project needs.
- All our images are based on [minideb](https://github.com/bitnami/minideb) a minimalist Debian based container image which gives you a small base container image and the familiarity of a leading Linux distribution.
- All Bitnami images available in Docker Hub are signed with [Docker Content Trust (DCT)](https://docs.docker.com/engine/security/trust/content_trust/). You can use `DOCKER_CONTENT_TRUST=1` to verify the integrity of the images.
- Bitnami container images are released on a regular basis with the latest distribution packages available.

## Supported tags and respective `Dockerfile` links

Learn more about the Bitnami tagging policy and the difference between rolling tags and immutable tags [in our documentation page](https://docs.bitnami.com/tutorials/understand-rolling-tags-containers/).


- [`1`, `1-scratch`, `1.0.2`, `1.0.2-scratch-r5`, `latest` (1/scratch/Dockerfile)](https://github.com/bitnami/bitnami-docker-rmq-default-credential-updater/blob/1.0.2-scratch-r5/1/scratch/Dockerfile)

Subscribe to project updates by watching the [bitnami/rmq-default-credential-updater GitHub repo](https://github.com/bitnami/bitnami-docker-rmq-default-credential-updater).

## Get this image

The recommended way to get the Bitnami rmq-default-credential-updater Docker Image is to pull the prebuilt image from the [Docker Hub Registry](https://hub.docker.com/r/bitnami/rmq-default-credential-updater).

```console
$ docker pull bitnami/rmq-default-credential-updater:latest
```

To use a specific version, you can pull a versioned tag. You can view the [list of available versions](https://hub.docker.com/r/bitnami/rmq-default-credential-updater/tags/) in the Docker Hub Registry.

```console
$ docker pull bitnami/rmq-default-credential-updater:[TAG]
```

If you wish, you can also build the image yourself.

```console
$ docker build -t bitnami/rmq-default-credential-updater:latest 'https://github.com/bitnami/bitnami-docker-rmq-default-credential-updater.git#master:1/scratch'
```

## Why use a non-root container?

Non-root container images add an extra layer of security and are generally recommended for production environments. However, because they run as a non-root user, privileged tasks are typically off-limits. Learn more about non-root containers [in our docs](https://docs.bitnami.com/tutorials/work-with-non-root-containers/).

## Configuration

### Running commands

To run commands inside this container you can use `docker run`, for example to execute `default-user-credential-updater --help` you can follow the example below:

```console
$ docker run --rm --name rmq-default-credential-updater bitnami/rmq-default-credential-updater:latest --  --help
```

Check the [official RabbitMQ Default User Credential Updater documentation](https://github.com/rabbitmq/default-user-credential-updater) for more information.

## Contributing

We'd love for you to contribute to this container. You can request new features by creating an [issue](https://github.com/bitnami/bitnami-docker-rmq-default-credential-updater/issues), or submit a [pull request](https://github.com/bitnami/bitnami-docker-rmq-default-credential-updater/pulls) with your contribution.

## Issues

If you encountered a problem running this container, you can file an [issue](https://github.com/bitnami/bitnami-docker-rmq-default-credential-updater/issues/new). For us to provide better support, be sure to include the following information in your issue:

- Host OS and version
- Docker version (`docker version`)
- Output of `docker info`
- Version of this container
- The command you used to run the container, and any relevant output you saw (masking any sensitive information)

## License

Copyright &copy; 2022 Bitnami

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
