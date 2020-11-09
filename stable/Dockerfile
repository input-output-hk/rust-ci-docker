FROM circleci/rust:latest

LABEL org.opencontainers.image.vendor = "Input Output HK Limited"
LABEL org.opencontainers.image.description = "CI image for Jormungandr"

RUN sudo apt-get update && \
    sudo apt-get install -y protobuf-compiler && \
    sudo apt-get clean

RUN cargo install cargo-audit && \
    rm -rf /usr/local/cargo/registry

RUN rustup component add clippy
