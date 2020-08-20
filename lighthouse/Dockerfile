FROM debian:buster-slim

RUN apt-get update && apt-get install -y --no-install-recommends \
  libssl-dev \
  ca-certificates \
  wget \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*
RUN wget https://github.com/sigp/lighthouse/releases/download/v0.2.6/lighthouse-v0.2.6-aarch64-unknown-linux-gnu.tar.gz
RUN tar -xvf lighthouse-v0.2.6-aarch64-unknown-linux-gnu.tar.gz

RUN mv lighthouse /usr/local/bin/
ENTRYPOINT []
