# Idris Alpine

[![Docker build status](https://img.shields.io/docker/build/ajhamwood/idris-alpine.svg)](https://hub.docker.com/r/ajhamwood/idris-alpine/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A docker image based on **Alpine Linux** for the **Idris** programming language.

Can be used like so:

    docker run --rm --name yourProject \
      -v $(pwd):/app -w /app -it ajhamwood/idris-alpine \
      ash -c 'idris source.idr -o compiled && ./compiled'