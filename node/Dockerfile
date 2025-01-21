FROM imbios/bun-node:1-22-slim AS base

# Install Taskfile
RUN  \
  apt-get update && apt-get install -y --no-install-recommends wget && \
  sh -c "$(wget -O- https://taskfile.dev/install.sh)" -- -d -b /usr/local/bin && \
  apt-get clean && rm -rf /var/lib/apt/lists /tmp/* /var/tmp/*
