FROM mcr.microsoft.com/devcontainers/javascript-node:20-bookworm

RUN apt-get update && \
    apt-get install -y --no-install-recommends git curl ca-certificates && \
    rm -rf /var/lib/apt/lists/*

RUN curl -fsSL https://bun.sh/install | bash \
 && ln -s /root/.bun/bin/bun  /usr/local/bin/bun \
 && ln -s /root/.bun/bin/bunx /usr/local/bin/bunx
