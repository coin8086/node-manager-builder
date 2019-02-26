# Node Manager Builder

It's for building [HPC Pack Linux Node Manager](https://github.com/coolmay/whpc-linux-communicator). 

It provides two ways to build that: build on a Ubuntu machine directly, or build in docker. 

## Get Source Code

Whichever way you use, you need to prepare the source code before. Make sure it has the following directory structure:


```
.
├── build-in-docker
├── build-native
├── docker-image
└── src
    ├── cpprestsdk
    ├── evancasa -> cpprestsdk
    ├── evanspdlog -> spdlog/
    ├── spdlog
    └── whpc-linux-communicator

```

*Note: do use a release version of cpprestsdk! Check releases by `git tag`* 

## Build Directly

Use `build-native` to build directly on an Ubuntu machine. You'd better setup your machine as the `Dockerfile` under `docer-image` does.

## Build in Docker

Make a Docker image by the file under `docker-image`. Name it `nm-builder`. Then use `build-in-docker` to build it.

## Get Build Result

Build result will be put at `release` dir, with all dependencies, be it glibc, boost, or cpprestsdk.

## TODO

* Push the docker image so you don't need to build one and only pull it from anywhere.
* Get *correct* source code automatically
