This repository provides Dockerfiles for container images used to
build Jormungandr and other Rust components in
[CircleCI](https://circleci.com/) workflows.

We build images under two tags:

- `stable`: based on the [official CircleCI image][circleci-image]
- `nightly`: based on the [official Rust nightly image][nightly-image]

[circleci-image]: https://circleci.com/docs/2.0/circleci-images/#rust
[nightly-image]: https://hub.docker.com/r/rustlang/rust

The Protobuf compiler is installed into both images.
