# tfsec_docker

This is a Docker image that contains [tfsec](https://github.com/liamg/tfsec/),
an excellent tool written by [Liam Galvin](https://github.com/liamg) for
performing static code analysis on Terraform code.

This image will be rebuilt daily thanks to the fine folks at 
[github](https://github.com/), [Travis CI](https://travis-ci.org/), and
of course, [Docker Hub](https://hub.docker.com/).

## Usage

### Build image

To build your own image:

```sh
docker build -t tfsec .
```

### Run tfsec

To use the daily build from Docker Hub:

```sh
docker run --rm -it -v "$(pwd):/workdir" wesleydeanflexion/tfsec .
```

To run your own image:

```sh
docker run --rm -it -v "$(pwd):/workdir" tfsec .
```

