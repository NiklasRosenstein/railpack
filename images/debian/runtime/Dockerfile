FROM debian:bookworm-slim

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y \
    ca-certificates \
    pkg-config \
    openssl \
    && rm -rf /var/lib/apt/lists/*

RUN groupadd -g 1000 railpack && useradd -u 1000 -g railpack -m railpack
