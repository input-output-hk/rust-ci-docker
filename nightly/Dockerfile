FROM rustlang/rust:nightly

LABEL org.opencontainers.image.vendor = "Input Output HK Limited"
LABEL org.opencontainers.image.description = "CI image for Jormungandr (nightly Rust)"

RUN apt-get update && \
    apt-get install -y protobuf-compiler && \
    apt-get clean
