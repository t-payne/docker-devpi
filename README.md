# docker-devpi

[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/coatl-dev/docker-devpi/coatl.svg)](https://results.pre-commit.ci/latest/github/coatl-dev/docker-devpi/coatl)
![Docker Pulls](https://img.shields.io/docker/pulls/coatldev/devpi)

Docker image with `devpi-client`, `devpi-server` and `devpi-web` pre-installed
using [`python:3.12-slim`].

## Supported tags

- [`6`, `6.12`, `6.12.0`, `latest`] - Comes with `devpi-server` 6.12.0,
  `devpi-web` 4.2.2 and `devpi-client` 7.0.3.
- [`6.11`, `6.11.0`] - Comes with `devpi-server` 6.11.0, `devpi-web` 4.2.2 and
  `devpi-client` 7.0.3.
- [`6.10`, `6.10.0`] - Comes with `devpi-server` 6.10.0, `devpi-web` 4.2.1 and
  `devpi-client` 7.0.2.
- [`6.9`, `6.9.2`] - Comes with `devpi-server` 6.9.2, `devpi-web` 4.2.1 and
  `devpi-client` 6.0.5.
- [`6.9.1`] - Comes with `devpi-server` 6.9.1, `devpi-web` 4.2.1 and
  `devpi-client` 6.0.5.
- [`6.9.0`] - Comes with `devpi-server` 6.9.0, `devpi-web` 4.2.0 and
  `devpi-client` 6.0.4.

## How to use this image

To run locally:

```bash
docker run \
  --name devpi-server \
  --detach \
  --publish 3141:3141 \
  --volume /tmp/devpi:/devpi \
  --env DEVPI_PASSWORD=password \
  coatldev/devpi:6.12.0
```

[`6`, `6.12`, `6.12.0`, `latest`]: https://github.com/coatl-dev/docker-devpi/blob/6.12.0/Dockerfile
[`6.11`, `6.11.0`]: https://github.com/coatl-dev/docker-devpi/blob/6.11.0/Dockerfile
[`6.10`, `6.10.0`]: https://github.com/coatl-dev/docker-devpi/blob/6.10.0/Dockerfile
[`6.9`, `6.9.2`]: https://github.com/coatl-dev/docker-devpi/blob/6.9.2/Dockerfile
[`6.9.1`]: https://github.com/coatl-dev/docker-devpi/blob/6.9.1/Dockerfile
[`6.9.0`]: https://github.com/coatl-dev/docker-devpi/blob/6.9.0/Dockerfile
[`python:3.12-slim`]: https://github.com/docker-library/python/blob/HEAD/3.12/slim-bookworm/Dockerfile
