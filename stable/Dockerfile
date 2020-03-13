FROM cimg/rust:1.42

LABEL org.opencontainers.image.vendor = "Input Output HK Limited"
LABEL org.opencontainers.image.description = "CI image for Jormungandr"

RUN sudo apt-get update && \
    sudo apt-get install -y pkg-config libssl-dev protobuf-compiler && \
    sudo apt-get clean

RUN cargo install cargo-audit && rm -rf /home/circleci/.cargo/registry
