# Maven Buildkite example

This example uses [Maven](http://maven.apache.org) to run tests, build a package, and then uploads the package as a [Buildkite artifact](https://buildkite.com/docs/builds/artifacts) using the current stable [Buildkite Agent](https://buildkite.com/docs/agent). You just need `mvn` installed in your `$PATH`.

This example also works on the beta Buildkite Agent using [the Docker Compose plugin](https://github.com/buildkite-plugins/docker-compose-buildkite-plugin) to run Maven in [the Maven Docker container](https://hub.docker.com/_/maven/), which works great on the [Elastic CI Stack for AWS](https://github.com/buildkite/elastic-ci-stack-for-aws).

![Maven package build with tests](https://user-images.githubusercontent.com/14028/30009989-ef3a8868-916f-11e7-9946-3a613a157f53.png)

![Maven uploaded target artifacts](https://user-images.githubusercontent.com/14028/30009990-ef961868-916f-11e7-84b7-3ab90be83f3c.png)

See the full [Getting Started Guide](https://buildkite.com/docs/guides/getting-started) for step-by-step instructions on how to get this running, or simply click the following link to add this project to Buildkite:

[![Add to Buildkite](https://buildkite.com/button.svg)](https://buildkite.com/new)

## License

See [LICENSE.md](LICENSE.md) (MIT)
