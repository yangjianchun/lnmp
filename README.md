**[中文说明](README_CN.md)**

## Introduction

lnmp-docker is a base on docker-compose service choreography repository that allows you to quickly build a complete swoft environment based on docker containerization.

## Environmental Requirements

1. docker engine release 17.06.0+

2. [docker-compose release 1.14.0+](https://github.com/docker/compose/releases/tag/1.14.0)

**reference to: [Compose file version 3 reference](https://docs.docker.com/compose/compose-file/#reference-and-guidelines)**

## Usage

## docker for linux

Here, if your operating system is `Linux`, then **recommends** to modify several configuration items under `.env`.

- APP_CODE_PATH_CONTAINER_MODE=:cached

```
docker-compose -f docker-compose.yml up
```
## License

Swoft is an open-source software licensed under the [LICENSE](LICENSE)
