# Buildkite Maven Example

[![Build status](https://badge.buildkite.com/aab023f2f33ab06766ed6236bc40caf0df1d9448e4f590d0ee.svg?branch=main)](https://buildkite.com/buildkite/artifact-example)

This repository is an example of testing and packaging a [Maven](http://maven.apache.org) project using [Buildkite](https://buildkite.com).
It demonstrates how to run unit tests, build a JAR file, and upload it as a [Buildkite artifact](https://buildkite.com/docs/builds/artifacts).

👉 **Live pipeline:** [buildkite.com/buildkite/maven--example](https://buildkite.com/buildkite/maven-example)

---

## How it works

This example:
- Uses Maven to run tests and build a package.
- Uploads the resulting JAR file as a Buildkite artifact.
- Runs on either:
  - A local agent with `mvn` in your `$PATH`, or
  - A Docker container via [the Docker Compose Buildkite Plugin](https://github.com/buildkite-plugins/docker-compose-buildkite-plugin), useful on the [Elastic CI Stack for AWS](https://github.com/buildkite/elastic-ci-stack-for-aws).

---

## Requirements

- A Buildkite agent
- Either:
  - Maven (`mvn`) installed on your agent machine, **or**
  - Docker + Docker Compose for the container-based setup

---

## To try it yourself

Clone this repo and run the tests locally:

```bash
mvn test

## License

See [LICENSE.md](LICENSE.md) (MIT)
