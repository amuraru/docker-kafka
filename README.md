# Kafka docker image

`amuraru/kafka` docker image build configuration.

A new `kafka-*` tag created in this repo triggers the image build and push to [ghcr.io/amuraru/kafka](https://github.com/amuraru/docker-kafka/pkgs/container/kafka) github docker registry.

Tags should be `<scala_version>-<kafka_version>` e.g `2.13-2.8.1`

# Upstream base

This is based on [wurstmeister/kafka-docker](https://github.com/wurstmeister/kafka-docker) with the following additions:
1. Use `openjdk 17` in order to support container based resource monitoring
2. Use custom `log4j.properties` to get all kafka logs to stdout only
