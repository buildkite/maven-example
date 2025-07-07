# Buildkite Maven Example

[![Build status](https://badge.buildkite.com/a947f64837044296a1ea4394819872e0544a4647a3400e6634.svg?branch=main)](https://buildkite.com/buildkite/maven-example/builds/latest?branch=main)
[![Add to Buildkite](https://img.shields.io/badge/Add%20to%20Buildkite-14CC80)](https://buildkite.com/new)

This repository is an example of testing and packaging a [Maven](http://maven.apache.org) project using [Buildkite](https://buildkite.com).
It demonstrates how to run unit tests, build a JAR file, and upload it as a [Buildkite artifact](https://buildkite.com/docs/builds/artifacts).

👉 **See this example in action:** [buildkite.com/buildkite/maven-example](https://buildkite.com/buildkite/maven-example/builds/latest?branch=main)

See the full [Getting Started Guide](https://buildkite.com/docs/guides/getting-started) for step-by-step instructions on how to get this running, or try it yourself:

[![Add to Buildkite](https://buildkite.com/button.svg)](https://buildkite.com/new)

<a href="https://buildkite.com/buildkite/maven-example/builds/latest?branch=main">
  <img width="2400" alt="Screenshot of example pipeline build page" src=".buildkite/screenshot.png" />
</a>

<!-- docs:start -->

## How it works

This example:
- Uses Maven to run unit tests and build a JAR package
- Uploads the JAR file as a [Buildkite artifact](https://buildkite.com/docs/builds/artifacts)
- Runs inside Docker using the [Docker Compose Buildkite Plugin](https://github.com/buildkite-plugins/docker-compose-buildkite-plugin), or on a local agent with `mvn` in your `$PATH`

It also works on the [Elastic CI Stack for AWS](https://github.com/buildkite/elastic-ci-stack-for-aws).

<!-- docs:end -->

## License

See [LICENSE.md](LICENSE.md) (MIT)