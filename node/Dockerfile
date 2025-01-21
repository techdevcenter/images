FROM imbios/bun-node:1-22-slim AS base

RUN \
  apt-get update && apt-get install -y wget && \
  apt-get clean && rm -rf /var/lib/apt/lists /tmp/* /var/tmp/*

RUN \
  sh -c "$(wget -O- https://taskfile.dev/install.sh)" -- -d -b /usr/local/bin
