# Buildkite Maven Example

[![Build status](https://badge.buildkite.com/a947f64837044296a1ea4394819872e0544a4647a3400e6634.svg)](https://buildkite.com/buildkite/maven-example)

This repository is an example of testing and packaging a [Maven](http://maven.apache.org) project using [Buildkite](https://buildkite.com).
It demonstrates how to run unit tests, build a JAR file, and upload it as a [Buildkite artifact](https://buildkite.com/docs/builds/artifacts).

👉 **See this example in action:** [buildkite.com/buildkite/maven-example](https://buildkite.com/buildkite/maven-example)

See the full [Getting Started Guide](https://buildkite.com/docs/guides/getting-started) for step-by-step instructions on how to get this running, or try it yourself:

[![Add to Buildkite](https://buildkite.com/button.svg)](https://buildkite.com/new)

<a href="https://buildkite.com/buildkite/maven-example/builds/latest?branch=main">
  <img width="2400" alt="Screenshot of example pipeline build page" src=".buildkite/screenshot.png" />
</a>

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

- A [Buildkite agent](https://buildkite.com/docs/agent)
- By default, this example uses Docker and Docker Compose.
  - ✅ You don’t need to install Java or Maven manually.
- **Optional:** If you prefer not to use Docker, you can run this pipeline on an agent with:
  - Java (JDK 8+)
  - [Maven](https://maven.apache.org) (`mvn`) installed and available in your `$PATH`

---

## To try it yourself

Clone the repo and run the tests locally:

```bash
docker-compose run maven mvn test
```

## License

See [LICENSE.md](LICENSE.md) (MIT)